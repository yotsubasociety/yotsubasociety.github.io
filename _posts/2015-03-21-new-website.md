---
layout: post
title: The Yotsuba Society's New Jekyll Website
tags: [blog, website, Yotsuba Society Bibliotheca Anonoma]
author: antonizoon
date: 2015-03-21 06:40:45
---

[The Bibliotheca Anonoma](http://github.com/bibanon/bibanon/wiki) has put together a brand new, [Jekyll](http://jekyllrb.com/) (and [Minimal Mistakes](http://mmistakes.github.io/minimal-mistakes))-based website for the [Yotsuba Society](http://yotsubasociety.org), which beats the rotting Drupal 7.x CMS it used to use. 

And don't worry, all the old pagelinks and downloads still work (we worked hard to make that possible), so no need to change your bookmarks.

## Situation

The [Yotsuba Society](http://www.yotsubasociety.org), recently discovered that their website was getting spam sites injected into their aging Drupal 7.x installation. 

Yes, with these messy, ancient CMS codebases, if you fail to update, security is like swiss cheese. It's a matter of time before your site gets exploited. And even if you think your site has nothing of value, it has valuable server space that spam sites can plaster their junk into.

![Imgur](http://i.imgur.com/j8Klw8T.png)

The admin's original plan was simply to shut down the site indefinitely, but that would have meant the total death of the Yotsuba Society. A great example that sometimes, even the archivists have to archived. So I instead recommended that they abandon the CMS system entirely, and replace it with a Static HTML engine (such as Jekyll). 

The CMS is often a necessary evil in large, account-based websites which implement forums, rich content, multiple posters, and such. However, by now the Yotsuba Society had significantly reduced it's operations, and was only using the CMS as a blog. Because Drupal 7 was now legacy code, it was starting to get spam ads injected into it to trick some poor saps.

Not everything has to be a giant Wordpress/Drupal/Joomla site. If you're only pushing information in a blog and some pages, perhaps with a few Disqus comments on the side, all you need is a static HTML engine, such as [Jekyll](http://jekyllrb.com/).

* **No more complex interfaces to wrestle with.** Just write a page and push (via FTP or Git).
* **No more bloated WYSIYWG editors.** Just write in Markdown syntax, it's easy to learn and has massive potential. Dump YouTube embed codes in, dump internal image links, and be done with it.
* **No more security issues.** Bloated CMS systems, with their accounts and SQL injection vulnerabilities, offer a massive attack surface, especially if it's not well updated. With Static HTML, there's nothing for attackers to attack, other than the web server admin console.
* **Static HTML uses significantly fewer resources.** You don't need a PHP engine or SQL Database to generate pages on the fly anymore. The HTML pages are pregenerated on the author's computer, and just thrown at the viewer. In fact, you can serve them for free via Github Pages (which allows you to use your same ol' custom domains).

And yes, Static HTML engines support comments too, via [Disqus.](https://help.disqus.com/customer/portal/articles/472138-jekyll-installation-instructions)

### The Journey

Creating this website was a massive undertaking, needed patching of several import scripts, and took quite a bit of time to get working. But it's a great example to follow if your website is stuck on a rotting Drupal 7.x CMS, just like we were.

[Click here to read about the amazing adventure.](http://blog.bibanon.org/basc/migrating-to-jekyll-from-drupal/)
