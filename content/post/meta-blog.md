---
author: "Frankie Sanzica"
title: "Meta: Blog"
date: 2019-07-22
description: "Blog"
draft: false
tags: ["meta"]
series:  ["meta"]
---

* Hugo: https://gohugo.io/
* Theme: https://themes.gohugo.io/type/

Quickstart:

```
hugo new site blog.frankiesanzica.com
cd blog.frankiesanzica.com
git init
git submodule add https://github.com/digitalcraftsman/hugo-type-theme themes/hugo-type-theme
hugo new posts/my-first-post.md
hugo server -D
http://localhost:1313
```

## Hosting

* Netlify: https://www.netlify.com/
* https://gohugo.io/hosting-and-deployment/hosting-on-netlify/
* Point *blog.frankiesanzica.com* to Netlify:

```
blog CNAME EXAMPLE-SITE-123456.netlify.com.
```