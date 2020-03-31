---
author: "Frankie Sanzica"
title: "Meta: How I built this website"
date: 2020-02-26
description: "How I build & host this website for FREE"
draft: false
tags: ["meta"]
series:  ["meta"]
---

*Prerequisites*:

* **Registrar**: Register *frankiesanzica.com* domain at [Google Domains](https://domains.google.com) ($12 /yr + **FREE** WHOIS privacy)
* **DNS/CDN**: Point DNS to [CloudFlare](https://cloudflare.com) nameservers (**FREE** CDN/HTTPS)
* **Email**: Add Zoho MX/TXT records to [Zoho](https://www.zoho.com/mail/) (**FREE** Email)

# Websites

1. **frankiesanzica.com**
    * GitHub Pages - Hosting/Version Control
    * Bootstrap - CSS Framework
    * Cloudflare - DNS/CDN/SSL
    * Zoho - Email
2. **blog.frankiesanzica.com**
    * Hugo - Static Site Generator
    * Netlify - Hosting/SSL/CDN/CI-CD"]
3. **docs.frankiesanzica.com**
    * MKDocs - Static Site Generator
    * Netlify - Hosting/SSL/CDN/CI-CD"]

# 1. FrankieSanzica.com 

## Bootstrap

* Bootstrap: https://getbootstrap.com/

##  GitHub Pages

* Setup *frankiesanzica.github.io* repo using [GitHub Pages](https://pages.github.com/) for **FREE** static hosting
* Add CNAME to GitHub for custom domain: https://github.com/FrankieSanzica/frankiesanzica.github.io/blob/master/CNAME
* Point *frankiesanzica.com* to GitHub IPs:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

# 2. Blog.FrankieSanzica.com

## Hugo

> To create my blog, I went with the open-source static site generator, [Hugo](https://gohugo.io/).  
> It is very easy to use and is written in [Go](https://golang.org/).
> I chose a simple, but full featured [theme](https://themes.gohugo.io/), [Type](https://themes.gohugo.io/type/) to get started.
> Here were my [Quick Start](https://gohugo.io/getting-started/quick-start/) steps assuming you are on a Mac:

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

## Netlify

> To host my blog, I went with [Netlify](https://www.netlify.com/).  It is a great Platform-as-a-service that provides hosting, custom domains, CDN, HTTPs, & CD for a [Jamstack](https://jamstack.org).  All [**FREE**](https://www.netlify.com/pricing/) for personal use.

> Hugo also provides a great tutorial on [hosting on Netlify](https://gohugo.io/hosting-and-deployment/hosting-on-netlify/).

### Point *blog.frankiesanzica.com* to Netlify

> Add the following CNAME record at [CloudFlare](http://cloudflare.com/):

```
blog CNAME EXAMPLE-SITE-123456.netlify.com.
```

# 3. Docs.FrankieSanzica.com 

## MkDocs
