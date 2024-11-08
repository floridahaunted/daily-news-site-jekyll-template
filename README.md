# Daily News Jekyll template

SEO-optimized and fully responsive Jekyll template for an entertainment news site ready for automated daily update and regeneration.

## mouse-auto-clickers.online

### A global info Hub dedicated to the mouse auto-clickers for Windows, Linux, macOS, PC, iPhone, Android

* Use This AutoClicker App to Rack Up Points on Idle Games
* The 5 Best Auto Clickers With Hotkeys for Windows
* The 5 Best Auto Clickers for Mac
* Teen hacked Roblox with iPhone
* Minecraft to lose VR support
* AutoClicker Memes Adventure on Youtube

[Demo](https://mouse-auto-clickers.online/)

Based on [Mediumish Jekyll Theme](https://www.wowthemes.net/mediumish-free-jekyll-template/) by WowThemes.net.

## Usage

Under Windows, after Jekyll installation done, simply run "\_\_serve.bat", it regenerates the whole site and listens as local http site at 0.0.0.0:4000.

NOTE. At very first time run "bundle install --standalone".

To deploy for production, take any text parser of your choice and replace all the entries of "http://0.0.0.0:4000/" to "https://yoursite.yourdomain/" in the file "_site\\assets\\js\\lunrsearchengine.js".

IMPORTANT. Update the file "_config.yml" according "yoursite.yourdomain" and other settings.

## Advantages

* No external dependencies. All the html/css/javascript stuff is 100% local.
* 100% fully responsive design, tested on a wide set of PCs, FullHD and 4K monitors, iPhones, Androids, etc.
* Built-in full text search engine works on all the pages and posts. After calling "\_\_serve.bat", file "lunrsearchengine.js" is updated correspondingly.
* Ready for automatic and semi-automatic content update. After a new post file in a Markdown format has been placed into a "_posts" folder, and "\_\_serve.bat" has been called, all the html pages and sitemap become updated correctly. You have to automate just a "_site" folder deployment to your nginx server.

## Format of a post file

Every new post file has a Markdown format, it should be placed in a "_posts" folder, and then, "\_\_serve.bat" should be called, and then, a "_site" folder should be deployed into your nginx directory.

Every new post file must have the following name: "YYYY-MM-DD-desired-http-path.md", then a corresponding URL "https://yoursite.yourdomain/desired-http-path/" will automatically appear
and will contain a publication date of "YYYY-MM-DD".

### Example Jekyll Front Matter header of "YYYY-MM-DD-desired-http-path.md"

```
---
layout: post
title:  "Your desired title"
description: "Your desired description"
image: assets/images/yourdesiredimage.jpg
toc: false
order: 1
---
````

Field "order" must contain a natural number. All the posts are sorted against "order" first, to appear on a site's Home page. Consider "order" as a kinda "importance".

We recommend that every "assets/images/yourdesiredimage.jpg" should have at least 1000px on the shortest side, should be saved in a common JPEG format with just 25% quality, and output file size should be less than 90Kb.
In other words, prepare high-resolution images but store them with poor JPEG quality, rather than prepare low-resolution images and store them with high JPEG quality.

* Don't forget to update the field "bdate" in your "_config.yml" file before call to "\_\_serve.bat". It is important for SEO, because "sitemap.xml" will be updated accordingly.

[Indeed!](https://profile.indeed.com/p/floridah-p5b9vzh)
