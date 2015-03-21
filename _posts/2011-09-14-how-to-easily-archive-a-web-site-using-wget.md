---
layout: post
title: How to Easily Archive a Web Site using Wget
author: colorado
permalink: /How_to_Easily_Archive_a_Web_Site/
redirect_from: /node/32/
created: 1316041975
---
<h2>How to Easily Archive a Web Site using Wget</h2>

In this tutorial I am going to be teaching you how to quickly and easily archive a Web site using Wget. Whilst it requires little interaction to start the process, it may take a long time to finish archiving, depending on both your local and the servers' connection speed. We'll also cover the basics of ignoring certain directories, which can be useful for a multitude of purposes (that I shall list later).

For starters, we're going to need to get a copy of the aforementioned application "Wget". If you're using GNU/Linux, you will already have Wget installed. However, if you're using Windows, we will have to install it manually.

<h3>Installing Wget on Windows</h3>

Installing Wget on Microsoft Windows is easy. Let's begin:

<ul><li>Download and install Wget from: http://downloads.sourceforge.net/gnuwin32/wget-1.11.4-1-setup.exe</li></ul>

...that's it!

</h3>A Test Run</h3>

Let's perform a test run. We're going to be downloading the file "reset.css" from one of my Web servers. Make sure to use the "cd" command to move into a directory you're comfortable downloading files into before continuing. Let's give it a go:

<b>GNU/Linux:</b>
$ wget http://notimeforlove.net/res/reset.css

<b>Windows (from within the Command Prompt):</b>
$ "C:\Program Files\GnuWin32\bin\wget.exe" http://notimeforlove.net/res/reset.css

The output should be something like this:

<blockquote>> david@colorado:~$ wget http://notimeforlove.net/res/reset.css
> --2011-09-14 16:53:33--  http://notimeforlove.net/res/reset.css
> Resolving notimeforlove.net (notimeforlove.net)... 178.33.84.77
> Connecting to notimeforlove.net (notimeforlove.net)|178.33.84.77|:80... connected.
> HTTP request sent, awaiting response... 200 OK
> Length: 1092 (1.1K) [text/css]
> Saving to: `reset.css'
> 
> 100%[=============>] 1,092       --.-K/s   in 0s
> 
> 2011-09-14 16:53:35 (146 MB/s) - `reset.css' saved [1092/1092]</blockquote>

We've learnt to use Wget to download a file, now let's get straight into the act of archiving a Web site.

<h3>Archiving a Web Site with Wget</h3>

Today we're going to archive notimeforlove.net.

Now, once again, use the "cd" command to move into the directory you'd like to store the archive. Then:

<b>GNU/Linux:</b>
$ wget -mk http://notimeforlove.net/

<b>Windows (from within the Command Prompt):</b>
$ "C:\Program Files\GnuWin32\bin\wget.exe" -mk http://notimeforlove.net/

The "-mk" means to do the following (copied from the manual):

<blockquote>>  -m
> --mirror
>     Turn on options suitable for mirroring.  This option turns on recursion and time-stamping, sets infinite recursion depth and keeps FTP directory listings.  It is
>     currently equivalent to -r -N -l inf --no-remove-listing.

> -k
> --convert-links
>     After the download is complete, convert the links in the document to make them suitable for local viewing.  This affects not only the visible hyperlinks, but any part
>     of the document that links to external content, such as embedded images, links to style sheets, hyperlinks to non-HTML content, etc.</blockquote>

...does that make sense? I hope so. Do a Google search for "Wget man page" if you need more information.

<h3>Ignoring Directories Whilst Archiving</h3>

We're going to try that one more time. However, we don't want to save any images, because they take up too much space, so we're going to prevent Wget from downloading anything from the "/artwork" directory.

<b>GNU/Linux:</b>
$ wget -mk -X/artwork http://notimeforlove.net/

<b>Windows (from within the Command Prompt):</b>
$ "C:\Program Files\GnuWin32\bin\wget.exe" -mk -X/artwork http://notimeforlove.net/

This will tell Wget to not download anything from "/artwork" (http://notimeforlove.net/artwork/). We can specify multiple directories by using commas to separate each directory. For example:

$ wget -mk -X/artwork,/res http://notimeforlove.net/

And that's all you need to know for basic archiving. For more information about Wget, what "-X" does or what else you can do with it, do a Google search for "Wget man page". Or, if you're lazy, just follow this link:

<blockquote>http://www.gnu.org/software/wget/manual/wget.html</blockquote>

Enjoy, and happy archiving. If you'd rather help from a person, talk to Colorado in #YotsubaSociety.
