+++
title = "Reading"
date = "2025-09-07"
lastmod = "2026-05-29"
menu = "main"
weight = 70
description = "Recomendations on further reading"
+++

This page is for linking other sites/articles that I would recommend you read if
your interests and mine overlap.

## [Unreal Engine 6, Blueprint, and Verse, or: Capitalism’s Unmatched Innovative Potential for New and Exciting Hellscapes](https://medium.com/@quiggy/unreal-engine-6-blueprint-and-verse-or-capitalisms-unmatched-innovative-potential-for-new-and-65d1970635a2)

For anyone interested in programming language design, this offers a good vertical slice into Epic Games' fancy new scripting language. Written informally, it's also a very entertaining read for anyone with opinions about stuff like keywords, whitespace, and functional programming.

> "_Oh no_. If you’re like me, you already have some alarm bells going off in your head. For one, writing a custom language is rarely the correct solution for any engineering problem — language design is _hard_, and the reason “bad” languages like C++ or PHP or [insert your least favorite language] persist is because despite having deep problems they still do something better than the alternative. Something much bigger stood out to me from this initial section, though: Verse is _code_. In other words, Verse is _not_ visual scripting, and it does _not_ replace Blueprint. It’s doing a different thing, and if you work at a studio that relies on Blueprint to bridge the designer/programmer gap, too bad. Your designers need to learn Verse now."

---

## [Nitpicking the shell history scene in Tron: Legacy](https://www.chiark.greenend.org.uk/~sgtatham/quasiblog/tron-legacy/)

A fun mix of media analysis and technical explanation. If you're the type of person to pause movies when there's a computer on screen to pick apart what system they're using, I highly recommend reading. And the cherry on top, this isn't Hollywood technobabble gobbledygook! The majority of quirks in this scene have in-universe explanations! Also, extra points for using the word "squozen". 

> "I hoped this might be fun, interesting, and/or educational. It succeeded at all three, beyond my hopes! Instead of the half hour I’d guessed, we spent a whole day on it, on and off (exchanging Slack messages, in between other work), and squeezed a lot more juice out of it than I’d realised was there to be squozen. By the end of the exercise, I’d decided one of my own initial complaints was wrong (but found another to replace it), and I’d learned some new things myself. And I ended up more impressed than I’d started, with whoever constructed that screenshot."

---

## [You Should Never Be The Most Sycophantic Participant In A Conversation With A Chatbot](https://defector.com/you-should-never-be-the-most-sycophantic-participant-in-a-conversation-with-a-chatbot)

A case study in why the idea that LLMs will improve if you just write better prompts is inherently flawed. Bonus points for dunking on Marc Andreessen for being both a finance-brained ghoul and willfully ignorant of how LLMs work. 

> "Andreessen is creating—typing out and entering, but not into the chatbot—his own delusion. In trying to tell the chatbot not to hallucinate, he is scripting his own psychotic break. He is doing it because he is a huge dumbass. Don't expect Claude to tell him so."

---

## [how to make programming terrible for everyone](https://jneen.ca/posts/2026-03-27-how-to-make-programming-terrible-for-everyone/)

An evaluation of LLMs role in programming by the standards of a programming language, hearkening all the way back to code generation tools released in 1981. It similarly evaluates the role of abstractions in programming, both why they're helpful and harmful.

> "At what point is the user of a system doing capital-P Programming? Is Excel a programming language? What about The Last One? If scratch is a programming language, does clicking around Unreal Engine count? nginx.conf? What about the command-line flags of find?
>
> From my perspective, AI can be seen as an incredibly poorly designed computer language."

---

## [CCC vs GCC](https://harshanu.space/en/tech/ccc-vs-gcc/)

A comparison between GCC and Anthropic's Claude C Compiler. Very well written, and gives a great rundown on how compilers work. Also shows why being "technically correct" isn't good enough when developing a compiler.

> "GCC has been in development since 1987. That is close to 40 years of work by thousands of contributors. It supports dozens of architectures, hundreds of optimization passes and millions of edge cases that have been discovered and fixed over the decades. The optimization passes alone (register allocation, function inlining, loop unrolling, vectorization, dead code elimination, constant propagation) represent years of PhD-level research. This is one of the reasons why it’s ubiquitous.
>
> This is why CCC being able to compile real C code at all is noteworthy. But it also explains why the output quality is far from what GCC produces. Building a compiler that parses C correctly is one thing. Building one that produces fast and efficient machine code is a completely different challenge."

---

## [Deep dive into Turso, the "SQLite rewrite in Rust"](https://kerkour.com/turso-sqlite)

A lighter piece about a new database engine that aims to be compatible with SQLite while taking advantage of Rust's type system and memory safety. The author isn't a developer of SQLite, but they offer a nuanced perspective on why SQLite exists, why it's so widely used, and why a compatible rust-based database engine would be useful.

> "SQLite is probably the most deployed database in the world, with dozens of databases on any of your devices and is probably one of the most reliable piece of software in existence, with 590 times more tests than code (I know that tests are code, it's to simplify): ~92,053,100 lines of tests vs ~155,800 lines of code."

---

## [Where's the Shovelware? Why AI Coding Claims Don't Add Up](https://mikelovesrobots.substack.com/p/wheres-the-shovelware-why-ai-coding)

A great piece from a former AI optimist who became disillusioned with the
technology and its promises at a very basic, input/output level.

> "My argument: If so many developers are so extraordinarily productive using
> these tools, where is the flood of shovelware? We should be seeing apps of all
> shapes and sizes, video games, new websites, mobile apps,
> software-as-a-service apps — we should be drowning in choice. We should be in
> the middle of an indie software revolution. We should be seeing 10,000 Tetris
> clones on Steam."

---

## [Iconography of the X Window System: The Boot Stipple](https://matttproud.com/blog/posts/x-window-system-boot-stipple.html)

An extremely niche deep-dive on the origin and purpose of the X windowing
system's root window texture.

> "So why write about something that seems purely like an indulgence? Surely the
> stipple still lives with us today and requires no further discussion? Well, up
> until the early-2010s (at least on the Linux distributions I was using), this
> boot up scene was common to see — until it suddenly wasn’t."

---

## [I Am An AI Hater](https://anthonymoser.github.io/writing/ai/haterdom/2025/08/26/i-am-an-ai-hater.html)

The title's a bit harsh, I know, but this article _goes places_. Extremely
worthwhile idealogical critique of AI. Plus it's only like 2 pages long, go read
it!

> "Altman tells lies for money. And I’m glad they’re lies. Because the makers of
> AI aren’t damned by their failures, they’re damned by their goals. They want
> to build a genie to grant them wishes, and their wish is that nobody ever has
> to make art again"

---

## [Email is Easy](https://e-mail.wtf/)

Step right up and test your knowledge! Simply identify if the given email
address is valid or not! Discover intricacies of the RFC 5322 Internet Message
Format standard you never even asked for! Can't get enough? Try the
[JSdate](https://jsdate.wtf/) quiz from the same author and try to identify
valid JavaScript dates!

> "`normal(wtf␣is␣this?)@example.com`? Technically valid. Did you know emails
> could have comments? Anything (in parens) is a comment. Introduced in RFC 822,
> but made obsolete by RFC 5322."

---

## [Apple Rankings](https://applerankings.com/)

Yes, it is _technically_ a website rating different varieties of apples.
However, the writing style is practically burning with passion. This isn't some
"Apples Weekly" joint or Buzzfeed-tier ranking, this is for the real
apple-heads.

> "Oh how the mighty have fallen! Believe it or not, the coffee grinds in a
> leather glove known as “The Red Delicious Apple” was once a robust firebrand
> credited with reinventing the apple from mere cider-fruit into a full-fledged
> lunch-worthy sidepiece. It even won the Stark Brothers apple contest in 1894.
> Likely your great-grandma’s favorite apple, this once flavorful Prometheus has
> been mass-produced into desolation."

---

## [Coding Without a Laptop - Two Weeks with AR Glasses and Linux on Android](https://holdtherobot.com/blog/2025/05/11/linux-on-android-with-ar-glasses/)

The smartphone market has stagnated surprisingly fast in the last decade or so,
but this project shows the first novel way to package a portable computer since
the iPhone. All for ~$250 if you already have a decent android phone!

> "I do feel a little weird wearing these in public, but not that weird. They
> more or less pass for sunglasses, so the odd part is wearing sunglasses
> indoors and typing on a keyboard with nothing in front of you. I had couple
> people ask me about them, but they seemed to just think they were cool. One
> guy said he was going to buy a pair. That may be selection bias though; I'm
> sure some people thought I was an idiot."

---

## [Hell Is Overconfident Developers Writing Encryption Code](https://soatok.blog/2025/01/31/hell-is-overconfident-developers-writing-encryption-code/)

The main content of this article is very "shop talk" and impenetrable to the
layman, but the context makes it entertaining nonetheless. If you're the kind of
person to google every unfamiliar term, you'll definitely learn a thing or two.

> "I’ve seen people use md5($password) as their key derivation function for
> libsodium. I’ve seen people encrypt fields in a database, and then store the
> decryption key right next to the ciphertext. And then, in a stunning display
> of brilliance, they wrote decryption logic in SQL so they could query their
> database over encrypted fields. At least once, when reviewing an end-to-end
> encryption project that implemented cryptography in JavaScript intended to run
> in the web browser, my question of “how do you know which public key to
> trust?” was answered with something shaped like, “Oh, we just store those in
> MySQL and fetch them from the server.”"
