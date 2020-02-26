---
author: "Frankie Sanzica"
title: "Meta"
date: 2019-06-29
description: "meta"
draft: true
tags: ["meta"]
series:  ["meta"]
---

# Opensource

1. Registrar
  * Google Domains
2. DNS/CDN
  * Cloudflare
  * Zoho
3. Personal Site
  * HTML
  * Bootstrap
4. Blog 
  * Hugo  
5. Hosting
  * GitHub Pages
  * Netlify

# Websites

## frankiesanzica.com

* GitHub Pages - Hosting/Version Control
* Bootstrap - CSS Framework
* Cloudflare - DNS/CDN/SSL
* Zoho - Email

## blog.frankiesanzica.com

* Hugo - Static Site Generator
* Netlify - Hosting/SSL/CDN/CI-CD---
author: "Frankie Sanzica"
title: "Meta Part III: Homepage"
date: 2019-07-21
description: "How I created my personal homepage.  Using Bootrap.  Using simple HTML & CSS.  Hosted for FREE on GitHub Pages."
draft: false
tags: ["meta"]
series:  ["meta"]
---

# Bootstrap

* Bootstrap: https://getbootstrap.com/

## Hosting

* Setup *frankiesanzica.github.io* repo using [GitHub Pages](https://pages.github.com/) for **FREE** static hosting
* Add CNAME to GitHub for custom domain: https://github.com/FrankieSanzica/frankiesanzica.github.io/blob/master/CNAME
* Point *frankiesanzica.com* to GitHub IPs:

```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

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

## 1. Registrar

*  Register *frankiesanzica.com* domain at [Google Domains](https://domains.google.com) ($12 /yr + **FREE** WHOIS privacy)

## 2. DNS/CDN

* Point DNS to [CloudFlare](https://cloudflare.com) nameservers (**FREE** CDN/HTTPS)

## 3. Email

* Add Zoho MX/TXT records to [Zoho](https://www.zoho.com/mail/) (**FREE** Email)
