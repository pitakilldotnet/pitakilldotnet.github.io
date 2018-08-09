+++
date = "2018-08-09T09:59:08-05:00"
description = "A path to clarify the development with: SSL, domain, docker and last but not least portable across machines and maybe colleagues in a specific project"
draft = true
slug = "portable-development-environment-with-docker"
summary = "A proposal for a volatile/portable environment with docker and valid domain. This is valid for any kind of language program, the language for this example is golang but is applicable with any other backend language"
tags = ["general", "docker", "ssl", "development", "portable", "volatile"]
title = "SSL, valid domain, docker, development"

+++
How manage the creation of a API in go (for example) with:

* Valid domain
* Valid SSL certificate
* Docker
* Portable

Some of you maybe know that access to the Geolocation in a browser requieres a valid domain, and valid SSL certificate to make all the queries without a problem, of course this is achievable in different forms, but if you want develop under the most similar environments that the staging and production envs, even if you do some kind of CI and CD, you need a technology like Docker, and the spec does not seem clear (at least to me) but with hope this Post is going to clarify some of these nuances.

### What do i understand for valid SSL and valid domain?

This is very simple indeed. A [FQDN (Fully Qualified Domain Name)](https://en.wikipedia.org/wiki/Fully_qualified_domain_name "FQDN (Fully qualified domain name)") with a SSL signed by a [CA (Certificate Authority)](https://en.wikipedia.org/wiki/Certificate_authority "CA (Certificate Authority)") trusted by the browsers currently most used. In simples words, a green lock in Chrome in the URL area.

This is important for multiple reasons, but for make some kind of petitions to different services is a key, e.g. the Geolocation needs a valid SSL and valid domain to be smooth in the API calls.