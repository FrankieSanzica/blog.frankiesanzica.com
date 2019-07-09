---
author: "Frankie Sanzica"
title: "Meta: How I Made This Site"
date: 2019-06-29
description: "How I made this site & blog utilizing a JAMstack. "
draft: false
tags: ["jamstack"]
series:  ["Meta"]
---

## 1. Registrar

*  Register *frankiesanzica.com* domain: https://domains.google.com ($12 /yr + **FREE** WHOIS privacy)

## 2. DNS/CDN

* Point DNS to CloudFlare nameservers: https://cloudflare.com (Free CDN/SSL)

## 3. Email

* Add Zoho MX/TXT records to CloudFlare: https://www.zoho.com/mail/ (Free Email)

## 4. Personal Site

* Bootstrap: https://getbootstrap.com/

## 5. Blog

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

### Personal Site

* Setup *frankiesanzica.github.io* repo using GitHub Pages: https://pages.github.com/ (Free static hositing)
* Add CNAME to GitHub for custom domain: https://github.com/FrankieSanzica/frankiesanzica.github.io/blob/master/CNAME
* Point *frankiesanzica.com* to GitHub IPs:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

### Blog

* Netlify: https://www.netlify.com/
* https://gohugo.io/hosting-and-deployment/hosting-on-netlify/
* Point *blog.frankiesanzica.com* to Netlify:

```
blog CNAME EXAMPLE-SITE-123456.netlify.com.
```
