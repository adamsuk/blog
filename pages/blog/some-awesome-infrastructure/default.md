---
title: 'Some Awesome Infrastructure'
slug: some-awesome-infrastructure
date: 30-03-2022
tags:
    - Ramblings
    - Tech
description: 'After some major upgrades to my site and some long overdue links with my self hosted setup I wanted to document some of my cool setup.'
cover_image: ''
published: true
---

Hey so I've got every intention of this page being the single point of truth about my entire infrastructure setup. I'm a little worried this will

1. Miss some vital stuff
2. Get outdated quick

So instead of promising something I'll hate producing and updating I'll give a good overview here and make sure to include links to repositories and useful external sources.

Where to begin. I guess the simplest place is my domain [sradams.co.uk](https://github.com/adamsuk/sradams-co-uk-content).

* Domain bought from Google Domains
* DNS outsourced to CloudFlare
* Frontend Next.js site hosted via SaaS
* Backend subdomains a mixture of SaaS and self-hosted

### SaaS
I love nothing more than having a good excuse trial out a SaaS platform and integrate it into my ecosystem.
- Vercel - Frontend is dead simple, I love it. I've been using Netlify for a while now but like most things on my personal site I wanted to branch out, so my sites hosted on Vercel. It works a charm with Next.js (given it's made by the same company) and I've never had a problem or need to change it. Great SaaS!
- Heroku - My backend services are a little more complicated. For apps I've created like my [podcast API](https://github.com/adamsuk/podcast-express-api) I utilise Heroku, again AMAZING!

### Self Hosted
For established and prebuild containers I self host on a HP Microserver Gen8. I've been playing around with containers for close to a decade now and upgraded to a dedicated server setup 5 years ago (prior to that I repurposed old desktops). Before moving over to web dev as a job I used it for Plex on my local network, digitising my music and film catalogues. These days there's a lot more which you can find here. I've always maintained a boundary with my own services, preferring the GitHub integrations and DevOps that comes with it.

As I alluded to I host a fair amount [running locally](https://github.com/adamsuk/docker) and carefully open the door to my private network for specific services:
* [Plex](https://github.com/adamsuk/docker/blob/main/plexms/docker-compose.yml) - used less and less these days now streaming services are stepping up but during my wire cutting days I set it up and it came in useful during lockdown. No DNS records needed as it's all registered and routed through Plex with auth.
* [Nextcloud](https://github.com/adamsuk/docker/blob/main/nextcloud/docker-compose.yml) - self hosted cloud storage. Used more and more as a form of automated backups for things like photos on mobile devices but also extremely useful for sharing files. I used this for a long time on LAN but recently opened it up on a subdomain and love the flexibility.
* [Ubooquity](https://github.com/adamsuk/docker/blob/main/configs/docker-compose.yml) - an awesome comic and ebook service. Not utilised as much as I'd like but opened up via a subdomain on the off chance I want to read something whilst away.
* [Grav](https://github.com/adamsuk/docker/blob/main/grav/docker-compose.yml) - a recent addition but utilised and integrated into my blog on sradams.co.uk/blog. It's also available on a subdomain but I'm currently utilising it as a headless CMS and it's working a treat!
* [SWAG](https://github.com/adamsuk/docker/blob/main/swag/docker-compose.yml) - a prebuilt NGINX setup for enabling reverse proxies from docker networks. LOVE IT. Without it I'd need to rethink how I'd expose these services.