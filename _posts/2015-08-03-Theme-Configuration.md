---
layout: post
title:  "Theme Configuration"
date:   2015-08-03 15:00:00
categories: jekyll theme
excerpt: Requisites, Versions, installation, configuration...
---

## Pre-Requisites

I am not using `gem gh-pages`. Keeping things synchronised with GitHub compatible versions just seems like an unnecessary limitation, I'll always have access to a machine that can build my site. So I just grabbed the latest stable version of Jekyll and Rouge.

``` bash
gem install jekyll -v 2.5.3
gem install rouge -v 1.9.1
```

If you do not have Ruby refer to these [instructions](http://jekyll-windows.juthilo.com/1-ruby-and-devkit/) to set things up on Windows.

These will remain the official versions for this theme until there is a reason to change. If you have other versions install that you do not want to remove, you can either just try it or make a gemfile and use [bundler](http://bundler.io/).


## A Note on Licence

Initially I had set this GPL. The issue with this is I'm not entirely sure how that would actually apply to a theme. So I switched to [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/).

I don't regard any visible content you create to be a part of the theme, so all you have to share is a repo of your modifications of the theme, not the whole blog/webiste you create. Also attribution from the repository readme is sufficient, you don't need to attribute from the site itself. 


## Theme Installation

If you're starting a new blog then you can just clone the whole repo and start from there.

If you want to update an existing blog:

 * Copy the `css` and `_sass` folders to get all my styles.
     - If this is all you want then manually copy the font links from `_includes/head.html`.
 * Copy `_include`, `_layouts_` and `index.html`.
     - `about.md` and `archive` are optional.
     - You must merge and missing entries from my `_config.yml` to your own.
     - The build settings part of the config is usually rather important.


## Configuration

Change everything in `_config.yml` to suit yourself. Please place a link back to my Github in your `readme.md`. It is also nice to credit the theme you built on in the footer but it is not necessary.