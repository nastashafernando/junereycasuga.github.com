---
layout: post
title: "Blogging in a Different Way"
description: ""
category: Blogs
tags: [web development, junerey casuga, blogging, jekyll, git, github]
---
{% include JB/setup %}

Bloggers usually use Blogging Platforms like [Wordpress](http://wordpress.com), [Tumblr](http://tumblr.com), [Blogger](http://blogger.com), and many more. But for some people, especially for those who are into programming were using [Jekyll](https://github.com/mojombo/jekyll).

From the description of Jekyll in GitHub, it is a simple, blog-aware, static site generator in Ruby. It takes a template directory (representing the raw form of a website), runs it through Textile or Markdown and Liquid converters, and spits out a complete, static website suitable for serving with Apache or your favorite web server. This is also the engine behind GitHub Pages, which you can use to host your project’s page or blog right from GitHub.

A lot of people were asking me how I do my blog site. So, I will show you a step-by-step procedure how I made my blog using Jekyll and hosted it through GitHub Pages.

1. Basically, you must have an account on [GitHub](http://github.com) because it is where you want to host your site.
<img src="/assets/images/github.png" title="GitHub" alt="GitHub" class="img-polaroid" />

2. After creating an account on GitHub, create a new repository and name it as <b>YOURUSERNAME</b>.github.com
<img src="/assets/images/new.png" title="New Repository" alt="New Repository" class="img-polaroid" />

3. Install <b>Jekyll-Bootstrap</b>. It is the first Jekyll blogging engine to support modular theming. To install Jekyll-Bootstrap on your machine, just type the codes below on your terminal:

		$ git clone https://github.com/plusjade/jekyll-bootstrap.git YOURUSERNAME.github.com
		$ cd YOURUSERNAME.github.com
		$ git remote set-url origin git@github.com:YOURUSERNAME/YOURUSERNAME.github.com.git
		$ git push origin master

4. After pushing the files into your repository, just wait GitHub do the magic. And your blog will be publicly running at [http://YOURUSERNAME.github.com](http://YOURUSERNAME.github.com)


Jekyll-Bootstrap is using the Twitter Bootstrap as its default theme. But the Twitter Bootstrap version its using is not updated. If you want to usethe latest version of Twitter Bootstrap, just download the latest version of Twitter Bootstrap from [http://twitter.github.com/bootstrap](http://twitter.github.com/bootstrap) and replace the old version with the new one. 

There you go! I hope I was able to help you developing your blog site using Jekyll. Let's blog in a different way! Cheers!