---
title: "Homelabbing isn't hard, it's just complicated"
params:
  icon: " "
date: 2026-01-12T10:45:52-05:00
publishDate: 2026-01-12T10:45:52-05:00
lastmod: 2026-01-12T10:45:52-05:00
tags:
  - blog
  - homelab
  - networking
categories: []
series: []
description: "Explanation and exploration of my homelabbing journey in a format that makes it easy to follow along"
draft: true
---

<!--markdownlint-disable MD025 MD033 MD013 MD036-->

Now, right off the bat, what the hell do I mean by "not hard, just complicated"? By that I mean homelabbing is something really easy to set up and do, provided you already have a truckload of preexisting knowledge about networking, remote administration, and Docker. It's ultimately plugging square pegs into square holes, finding out it doesn't fit, searching "square peg square hole not fitting" on StackOverflow and finding out there's a secret square hole you should be using because the obvious square hole on the front doesn't accept purple squares and this has been a problem since 1997, the secret square hole was a band-aid fix that should've been reworked years ago but now every square is built with the assumption that there are 2 slightly different square holes so fixing it now would do more harm than good.

That's ultimately what I mean by "not hard, just complicated". You're not making something from scratch, all the hard parts have already been developed, but to use them for your own ends you need to understand how they work at least a little bit. Not enough to write patches, just enough to look at an error message and know which part's broken. And that process begins with networking.

## Networking

Networking is an incredibly broad subject that can be easy to lose yourself in, but for our purposes we just need to consider how you want to access your services. All networked services run on HTTP "ports". The port number can be anywhere from 0 to 65535, and some services can use multiple ports. You can access any service simply by typing your lab's IP address followed by the port like so: `10.0.0.1:1234`. This IP is your **local** IP, meaning it's only accessible by devices connected to the same network. You can scan your local network for devices using `nmap` with the following arguments.

```bash
nmap -sP 192.168.1.0/24
```

This address is assigned by your router, and [different routers use different IP ranges](https://www.techspot.com/guides/287-default-router-ip-addresses/) for local IP addresses. You can find yours in whatever settings app you use or `fastfetch` if you're comfortable with the command line. If you aren't, you need to change that pretty soon because the most useful and flexible way to remotely access your lab is SSH.

### SSH

SSH is great. If you get into homelabbing, it will become your lifeline. Remote, root-level access to your machine is obviously incredibly powerful, which is why you'll want to do a few things to secure it first.

Before you can do anything, your lab has to be running the SSH Daemon[^1]. This is a good opportunity to get familiar with Systemd services. It's not necessary, you can technically just run `sshd` in a terminal and leave it open, but Systemd is a common way to manage these background processes.

```bash
sudo systemctl enable --now sshd.service
#Or, if you don't want sshd to run on startup, instead run
sudo systemctl start sshd.service
```

[^1]: The name "Daemon" actually comes from some nerds at MIT in 1963 who took inspiration from "Maxwell's Daemon", which is a physics thought experiment that gets its name from ancient Greek definition of Daemon: an "unknown superfactor". Essentially a catch-all term for the cause of phenomenon unexplainable by reason or divinity. They're just little guys that design snowflakes and shape clouds and tangle headphone cables. Sorry to get your hopes up, homelabbing does not involve Luciferian rituals.
