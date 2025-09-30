---
title: "Arch Linux Derivatives"
params:
  icon: "󰜡 "
date: 2025-09-10
publishDate: 2025-09-10
lastmod: 2025-09-10
tags:
  - linux
  - arch
categories: []
series: []
description: "An overview of Arch-derived Linux distributions"
draft: true
---

Arch Linux has a reputation for being a "difficult" distribution. I've written
previously about how that's not really something that needs to change, smoother
onboarding just isn't a part of the Arch Linux project. The appeal of Arch is
that it ships with basically no software. While the latest Ubuntu ISO is ~5.8
gigabytes, Arch's September 2025 ISO is just ~1.4 gigabytes. In fact, if you
look at the packages included as part of the base installation, you'll find a
very funny snippet to read on a website documenting a Linux distribution.

![List of dependencies defining an Arch Linux system. Linux itself is optional.](./images/linux-optional.png)

This design philosophy of build-it-yourself has lead to a number of pre-built
distributions downstream that offer more than a foundation. Not to say that
these are all "Arch but Easy", I'd liken it to using cake mix. You still have to
bake the rest of the cake, but you can outsource a few steps. That being said,
the same pitfalls apply here. You better REALLY trust Betty Crocker if you're
letting her make fundamental decisions about your cake. And in
[Betty Crocker's case](https://www.thekitchn.com/grandmas-arent-buying-boxed-cake-mix-23687784),
that's a bad idea.

##  Manjaro

Have ever wanted to run Arch while also being as plain as possible? Well, what
Ubuntu is to Debian, Manjaro is to Arch[^1]. Not nearly to the same extent,
Manjaro only established a company to offer enterprise support in 2019, but the
project overall follows Ubuntu's design philosophy of de-nerdifying the base
OS[^2]. For the most part, they've been doing that well enough for someone who
finds that appealing.

However, Manjaro comes with some [baggage](https://manjarno.pages.dev/). At the
time of writing, Manjaro has been on good behavior for a good while. 3 years is
probably long enough to say they're not going to DDoS the AUR anytime soon. My
main problem is just that there are better options these days if you want an
easier Arch experience. The
[archinstall](https://github.com/archlinux/archinstall) utility already provides
a built-in installer that a normal person can use, and there are better
distributions if all you want is a graphical installer.

##  EndeavourOS

This is the "user-friendly arch" option that nearly everyone recommends, and I'm
no different. I actually used to use this distro exclusively for installation
because I had a very fragile ego and didn't want a reminder that I wasn't smart
enough for vanilla Arch. Shaming myself into ricing aside, EndeavourOS is more
like a loose collection of utilities with very little in the way of core
modifications.

##  Artix

##  Garuda

## CachyOS

##  SteamOS

[^1]:
    The third pillar of linux distributions, Fedora, actually follows the
    opposite pattern. Red Hat Enterprise Linux was the base, and as the name
    would imply, it was used for enterprise stuff. Fedora is the nerd-ified
    version.

[^2]:
    I vividly recall a bit of documentation insisting against calling Manjaro
    "easy arch linux" but their
    [current docs](https://wiki.manjaro.org/index.php/About_Manjaro) are very
    open about user-friendliness being their main goal, so either that changed
    or I imagined it. Probably the latter, I was in a rough spot when I first
    tried Manjaro and my memory is patchy. Anyway, thanks for reading this
    footnote, you're a real one.
