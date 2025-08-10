---
title: "Hosting a Mastodon Server on Arch Linux"
params:
  icon: " "
date: 2025-08-05T13:13:57-04:00
publishDate: 2025-08-05T13:13:57-04:00
lastmod: 2025-08-05T13:13:57-04:00
tags:
  - blog
  - webdev
  - selfhost
  - fediverse
categories: []
series: []
description:
  "Tutorial for setting up a mastodon server on a local machine running Arch
  Linux."
draft: true
---

First off, let's get one thing out of the way. You probably shouldn't do this.
There are already a ton of guides on how to host Mastodon on Debian-based
distros. If you're doing this on a fresh machine, go with Ubuntu 22.04 and use
the [official guide](https://docs.joinmastodon.org/admin/prerequisites/). Arch
isn't a great server operating system. Its whole deal is being lightweight and
getting updates to the user as fast as possible. Servers need over a terabyte to
be useful and they don't update unless it's necessary. I only did this because I
know how to administer Arch and I already had a homelab running Arch with a few
services. Regardless, if you aren't willing to switch, here's what you need to
do.

## Prerequisites
