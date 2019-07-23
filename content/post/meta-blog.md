---
author: "Frankie Sanzica"
title: "Meta: Blog"
date: 2019-07-22
description: "Blog"
draft: false
tags: ["meta"]
series:  ["meta"]
---

# Hugo

To create my blog, I went with the open-source static site generator, [Hugo](https://gohugo.io/).  It is very easy to use and is written in [Go](https://golang.org/).

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

### Add theme:

```
git submodule add https://github.com/digitalcraftsman/hugo-type-theme themes/hugo-type-theme
```

### Add first post:

```
hugo new posts/my-first-post.md
```

### View on local test server:

```
hugo server -D
```

http://localhost:1313

## Hosting

To host my blog, I went with [Netlify](https://www.netlify.com/).  It is a great Platform-as-a-service that provides hosting, CDN, SSL, & CI/CD for a [Jamstack](https://jamstack.org).  

Hugo also provides a great tutorial on [hosting on Netlify](https://gohugo.io/hosting-and-deployment/hosting-on-netlify/)

### Point *blog.frankiesanzica.com* to Netlify:

```
blog CNAME EXAMPLE-SITE-123456.netlify.com.
```