# The Virgo Website
Welcome to The Virgo Website. The following text explains how the website is structured and also contains steps in 
order to amend its content.

### Creating Pages
A page file **MUST** be in the ````root```` directory. You can create a folder and add all the relevant posts for 
the corresponding page.

The simplest way of creating a new page is to add an HTML file with a suitable layout and front matter.

* Layouts (in ````_layouts```` directory): Layouts are templates that wrap around your content. They allow you to have the 
source code for your template in one place so you don’t have to repeat things like your navigation and footer on 
every page.

* Front matter: The front matter must be the first thing in the file and must take the form of valid YAML set between 
triple-dashed lines. Between these triple-dashed lines, you can set predefined variables or even create custom ones 
of your own. These variables will then be available to you to access using Liquid tags both further down in the file 
and also in any layouts or includes that the page or post in question relies on.

For example:

```

---
layout: page
title: "Virgo Meetings"
image: /assets/images/Meetings.jpg
---
```
### Creating Posts
A post file **MUST** be in the ````_posts```` directory and **MUST** have a name with the following format: 
year-month-day-title.markdown

All posts must begin with front matter which is typically used to set a layout or other meta data (see below)

For example:

```

---
layout: post
title: "The Hydrangea Project"
date: 2017-06-14
description: "A suite of 24 cosmological hydrodynamic zoom-in simulations of massive galaxy clusters."
image: /assets/images/Hydrangea.png
tags: [Hydrangea, GADGET]
---
```
### Assets
The ````assets```` folder **MUST** be in the ````root```` directory. 

Any css, images, files, js or videos are placed in there. Then, from within any post or page, they can be linked to 
using the site’s root as the path for the asset to include.

### Source Code
Below you can find the source code:

```
.
├── _assets
|   ├── js
|   └── scss
├── _includes
|   ├── contact.html
|   ├── disqus.html
|   ├── footer.html
|   ├── formcarry.html
|   ├── head.html
|   ├── header.html
|   ├── navigation.html
|   ├── pagination.html
|   ├── post-card.html
|   ├── share.html
|   ├── social.html
|   └── subscribe_form.html
├── _layouts
|   ├── about.html
|   ├── compress.html
|   ├── default.html
|   ├── index.html
|   ├── page.html
|   ├── post.html
|   └── tag.html
├── _plugins
├── _site
├── assets
|   ├── css
|   ├── files
|   ├── images
|   ├── js
|   └── videos
├── Page_About
|   ├── About.html
├── Page_Codes
|   ├── _posts
|   └── Codes.html
├── Page_Data
|   ├── _posts
|   └── Data.html
├── Page_Legacy
|   ├── _posts
|   └── Legacy.html
├── Page_Meetings
|   ├── _posts
|   └── Meetings.html
├── Page_Projects
|   ├── _posts
|   └── Projects.html
├── .eslintrc
├── .gitignore
├── .stylelintrc
├── 404.html
├── _config.yml
├── Gemfile
├── Gemfile.lock
├── gulpfile.js
├── index.html
├── package.json
├── README.md
├── style-guidle.html
└── subscribe.html

```
### Credits
This website has been built using Jekyll (https://jekyllrb.com) and specifically the Barber Jekyll theme, a blog 
theme for Jekyll built by Thomas Vaeth at Samesies (https://jekyllthemes.io/theme/barber)