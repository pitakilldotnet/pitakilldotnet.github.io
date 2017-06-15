+++
date = "2017-06-14T19:36:07-05:00"
description = ""
draft = false
tags = ["cloudflare", "gh-pages", "github", "free", "ssl", "custom-domain"]
title = "Moving this site to gh-pages with SSL for free"
slug = "hosting-in-github-custom-domain-for-free"

+++

This site was hosted in a VPS with 128 MB of RAM, and 10GB of disk space. So
far, so good. These specs are sufficient enough for run a
[hugo](https://gohugo.io/) server, a [nginx](https://nginx.org/en/) reverse proxy. And with [Let's
Encrypt](https://letsencrypt.org/) all is served with SSL.

Everything is smooth with this configuration, but in a near future (next month)
the plan with the VPS is over, and there is not possible to extend the contract
because the provider was acquired by a third and the product was outdated.

I really want to keep the site online and I don't want to pay $5 USD monthly for
a VPS in some provider like Digital Ocean, Rackspace or similar, a full year in
the last VPS was $12 USD, that was my first motivation to contract the VPS in
the first place.

Well, know with [github pages](https://pages.github.com/) with a custom domain, and with the awesomeness of
[Cloudflare](https://www.cloudflare.com/) you can place a project like this one.
With all the goodness like custom domain and SSL.

Basically you need:

+ A github account (Free)
+ A cloudflare account (Free)
+ A domain (Not free)
+ Some knowledge with DNS or just [Google](https://www.google.com.mx/search?q=github+pages+custom+domain+cloudflare+SSL&oq=github+pages+custom+domain+cloudflare+SSL&aqs=chrome..69i57j69i64.10971j0j1&sourceid=chrome&ie=UTF-8)
