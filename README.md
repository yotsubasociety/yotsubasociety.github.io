# Yotsuba Society Website

This is the new Jekyll/Minimal-Mistakes based Yotsuba Society website, created by the [Bibliotheca Anonoma](http://github.com/bibanon/bibanon/wiki) to replace the rotting Drupal 7.x website they used to use. Sometimes, even the archivists need to be archived.

And don't worry, all the old pagelinks and downloads still work (we worked hard to make that possible), so no need to change your bookmarks.

## Getting Started

Minimal Mistakes takes advantage of Sass and data files to make customizing easier. These features require Jekyll 2.x and will not work with older versions of Jekyll.

To learn how to install and use this theme check out the [Setup Guide](http://mmistakes.github.io/minimal-mistakes/theme-setup/) for more information.

### Creating/Editing a Blog Post

To create a new blog post, go to the `_posts/` folder in this repository and click the button pictured below to **Create a new file here**. 

![](https://camo.githubusercontent.com/8fdc501d6746c307ada3d168e5db7b8d1b12cd75/687474703a2f2f636c2e6c792f4c4c65302f6e65772d66696c652e6a7067)

Make sure to name your file, and follow the format of `2014-09-15-post-shortlink.md`. The words in the filename will be used as the shortlink, in this case `http://yotsubasociety.org/post-shortlink/`.

![](https://camo.githubusercontent.com/f4b2aa2358596bdaa11543d51c055da68927707a/687474703a2f2f636c2e6c792f4b77654c2f6e65772d66696c652d656469746f722e706e67)

Next, you need to create a FrontMatter section at the top. Just copy and paste the following and change fields as necessary: It is recommended that you specify some categories. Check the [Jekyll FrontMatter documentation](http://jekyllrb.com/docs/frontmatter/) for more info.

```yaml
---
layout: post
title: "This is your Blog Title, Change this"
excerpt: "Write a short description of your post here, this will be displayed as a preview."
tags: [blog, example]
category: "Example Category"
modified: 2014-09-15 14:40:45
---
```

> **Note:** Alternatively, to edit an existing post, click the file in the `_posts/` folder, and click **Edit** at the top right.

Now, you can write your blog post in Markdown format, right below the FrontMatter. Check out Github's excellent [Markdown Tutorial](https://help.github.com/articles/markdown-basics/) to get a feel for this powerful markup language. 

When you're finished, make sure to write a description of your changes in the **Commit changes** section. Then, click the **green Commit Changes** button to post the page to the blog.

## Create and edit Pages

Jekyll can do much more than plain ol' blog posts. You can also make website pages, for [Articles](http://yotsubasociety.github.io/articles/) or [Briefings](http://yotsubasociety.github.io/briefings/).

To create a new page, go to the `pages/` folder in this repository and click the button pictured below to **Create a new file here**.

![](https://camo.githubusercontent.com/8fdc501d6746c307ada3d168e5db7b8d1b12cd75/687474703a2f2f636c2e6c792f4c4c65302f6e65772d66696c652e6a7067)

Make sure to name your file, and follow the format of `2014-09-15-page-shortlink.md`. The words in the filename will be used as the shortlink, in this case `http://yotsubasociety.org/page-shortlink/`.

![](https://camo.githubusercontent.com/f4b2aa2358596bdaa11543d51c055da68927707a/687474703a2f2f636c2e6c792f4b77654c2f6e65772d66696c652d656469746f722e706e67)

Next, you need to create a FrontMatter section at the top. Just copy and paste the following and change fields as necessary: It is recommended that you specify some categories. Check the [Jekyll FrontMatter documentation](http://jekyllrb.com/docs/frontmatter/) for more info.

```yaml
---
layout: page
title: "This is your Page Title, Change this"
excerpt: "Write a short description of your page here, this will be displayed as a preview."
tags: [page, example]
category: page
modified: 2014-09-15 14:40:45
---
```

> **Note:** Alternatively, to edit an existing post, click the file in the `posts/` folder, and click **Edit** at the top right.

Now, you can write your page in Markdown format, right below the FrontMatter. Check out Github's excellent [Markdown Tutorial](https://help.github.com/articles/markdown-basics/) to get a feel for this powerful markup language. 

When you're finished, make sure to write a description of your changes in the **Commit changes** section. Then, click the **green Commit Changes** button to post the page to the blog.

Finally, you must link to the page before anyone will be able to access it. 

* If this page is an **Article**, [click the `articles.md` file at the top of the repository.](https://github.com/yotsubasociety/yotsubasociety.github.io/blob/master/articles.md)
* If this page is a **Briefing**, [click the `briefings.md` file at the top of the repository.](https://github.com/yotsubasociety/yotsubasociety.github.io/blob/master/briefings.md)

Then, click **Edit** at the top right. Then add a link to your new page in the bulleted list, as follows:

> **Note:** Make sure to create a relative link to the page. If your page's URL is `http://yotsubasociety.org/intro-to-ys/`, just link to `intro-to-ys/`.

```markdown
* [Introduction to Yotsuba Society](intro-to-ys/)
* [The Protochannel and the First Channel](ayashii-and-amezou/)
```

Now your page is available for the public to enjoy.
