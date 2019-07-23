---
author: "Frankie Sanzica"
title: "Meta: Blog"
date: 2019-07-22
description: "Blog"
draft: false
tags: ["meta"]
series:  ["meta"]
---

To create my blog, I went with the open-source static site generator, [Hugo](https://gohugo.io/).  It is very easy to use and is written in [Go](https://golang.org/).

I chose a simple, but full featured [theme](https://themes.gohugo.io/), [Type](https://themes.gohugo.io/type/) to get started.

Here were my quickstart steps assuming you are on a Mac:

1. Install:

```
brew install hugo
```

2. Start new site:

```
hugo new site blog.frankiesanzica.com
```

3. Add theme:

```
git submodule add https://github.com/digitalcraftsman/hugo-type-theme themes/hugo-type-theme
```

4. Add first post:

```
hugo new posts/my-first-post.md
```

5. View on local test server:

```
hugo server -D
```

http://localhost:1313

## Hosting

* Netlify: https://www.netlify.com/
* https://gohugo.io/hosting-and-deployment/hosting-on-netlify/
* Point *blog.frankiesanzica.com* to Netlify:

```
blog CNAME EXAMPLE-SITE-123456.netlify.com.
```