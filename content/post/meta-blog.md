---
author: "Frankie Sanzica"
title: "Meta Part IV: Blog"
date: 2019-07-22
description: "How I created my personal blog.  Quick Start to using Hugo, the static site generator.  Hosting for FREE on Netlify the Platform-as-a-service.  Pointing DNS at CloudFlare"
draft: false
tags: ["meta"]
series:  ["meta"]
---

# Hugo

To create my blog, I went with the open-source static site generator, [Hugo](https://gohugo.io/).  
It is very easy to use and is written in [Go](https://golang.org/).
I chose a simple, but full featured [theme](https://themes.gohugo.io/), [Type](https://themes.gohugo.io/type/) to get started.
Here were my [Quick Start](https://gohugo.io/getting-started/quick-start/) steps assuming you are on a Mac:

### Install

```
brew install hugo
```

### Start new site

```
hugo new site blog.frankiesanzica.com
```

### Add theme

```
git submodule add https://github.com/digitalcraftsman/hugo-type-theme themes/hugo-type-theme
```

### Add first post

```
hugo new posts/my-first-post.md
```

### View on local test server

```
hugo server -D
```

http://localhost:1313

## Hosting

To host my blog, I went with [Netlify](https://www.netlify.com/).  It is a great Platform-as-a-service that provides hosting, custom domains, CDN, HTTPs, & CD for a [Jamstack](https://jamstack.org).  All [**FREE**](https://www.netlify.com/pricing/) for personal use.

Hugo also provides a great tutorial on [hosting on Netlify](https://gohugo.io/hosting-and-deployment/hosting-on-netlify/).

### Point *blog.frankiesanzica.com* to Netlify

Add the following CNAME record at [CloudFlare](http://cloudflare.com/):

```
blog CNAME EXAMPLE-SITE-123456.netlify.com.
```