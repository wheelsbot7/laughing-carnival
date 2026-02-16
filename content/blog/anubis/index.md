---
title: "Anubis: The Best Captcha That Isn't"
params:
  icon: "󰒋 "
date: 2025-07-09T11:31:47-04:00
publishDate: 2025-07-17
lastmod: 2025-07-17
tags:
  - security
  - webdev
  - backend
categories: []
series: []
description:
  Explanation and recommendation of Anubis, a security solution for web servers
  designed to combat AI scrapers
draft: false
---

<!--markdownlint-disable MD029 MD030 MD013 MD022-->

If you're online enough to be reading this, I'm sure you're familiar with "Dead Internet Theory". It's mostly a cynical hypothesis that exists to cope about the lack of human connection on a platform specifically designed for it, but the sentiment behind it is more valid than you might think. The internet isn't dead or dying, but a greater proportion of it is being used by parasites. Bad actors[^1] that abuse the HTTP protocol for bad-faith reasons. Now that there's a market for reselling terabytes of other people's work, it's become harder to service actual requests.

## The Solution (Not Really)

The time-tested, industry-standard solution for this was Captchas. But those were always a flawed approach. Any image-based Captcha relied on the human brain's hyper-specialization with pattern recognition, but that was always a stopgap while machine vision advanced. JavaScript-based checks like Google's reCaptcha and Cloudflare's hCaptcha work better, but it's a constant arms race. New checks have to be implemented as fast as scrapers figure out how to spoof old ones. That's what makes Anubis special. It implements similar checks, but with the expectation that some scrapers will always slip through.

Instead of tightening the filter and increasing the chance of false positives, Anubis makes the site too computationally demanding for bots to access at scale. It does this by forcing all visitors to solve a small cryptographic hash function. This technique requires very little bandwidth, and means all heavy computation is done on the client's machine. Good-faith users will solve it once, access what they need, and leave, only wasting less than a second. Bots that are spamming HTTP requests like it's going out of business will waste hours and electricity solving thousands of hash functions.

## The Solution (Also Not Really but Better)

However, Anubis's true advantage is accessibility and convenience. No vision requirements means people relying on screen readers won't be affected. Additionally, the lack of a checkbox means if you have a fast enough computer, you might not even notice it. This unique approach makes Anubis a very attractive option for anyone concerned with how Captchas might impact user experience. Anecdotally, I'm always happy to see an Anubis check over a Cloudflare checkbox. I hope that with this understanding of how it works, you'll do the same.

Signing off: Wheelsbot

~~_The cute dog-girl art the default check shows also helps._~~

[^1]: Total tangent, but I never understood the term "bad actor" in this context. Like, what do you mean this high school theater kid is taking advantage of systems not designed for them? They should be singing Hamilton unprompted in the back of their school bus, making sure nobody will ever want to sit next to them, as is their (my) right.
