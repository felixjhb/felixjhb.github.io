---
title: Two Years Older     # Title of the post
date: 2023-06-28 19:00:00 +0100     # YYYY-MM-DD hh:mm:ss [+/-]TTTT where TTTT is the timezone
categories: [Non-Maths, Personal]   # Supports up to 2 categories
tags: [phd, university, planning]    # Supports arbitrarily many tags, tag names should always be lowercase
author: felixjhb    # author as defined in _data/authors.yml
toc: false      # enable table of contents on the right of the page?
comments: false     # enable user comments for this post?
math: true     # enable MathJAX processing for this post?
mermaid: false      # enable Mermaid diagram processing for this post?
excerpt_separator: <!--more-->  # Controls where content snippets stop
---

It's coming up to about two years since I started my PhD. The last year has been exceptionally busy for me - I've visited multiple conferences, given multiple talks, have a paper about to be published, and have caught COVID for what I suspect is the third time. <!--more--> As of last week, I have just completed my upgrade[^1] and am busy putting together big and exciting plans for what my next major research project is going to be, and how my thesis will look in about another two years time.

In the middle of this storm of big events and first milestones and bureaucracy, I take an opportunity to make myself a website and blog, and write what will (hopefully!) be the first of many posts.

Prior to setting this website up, I had been using [carrd.co](https://carrd.co) for about two years - an online service for creating simple billboard-style websites. Not enough to write blog posts or host complex content, but enough to point the curious user off in the right direction in search of greener pastures and heavier content. As my work progressed and I connected with other people, I feel that my needs quickly outgrew what was on offer. With the last few _big things of the year_ out of the way, I've finally made the transition to my own website[^2] hosted using [Github Pages](https://pages.github.com/).

Even better, this new platform makes it significantly easier to share technical content with the wider world. Even ignoring possibilities such as using WebAssembly to make animated or interactive content; having access to a platform with MathJax support is possibly the biggest and most immediate change. Research is great, but being able to communicate that research makes it valuable, and plugins like MathJax make talking technical details significantly smoother on my part.

\\[ 
    \frac{}{\Gamma \vdash \mathbb{N} \textrm{ type}} \qquad
    \frac{}{\Gamma \vdash 0 : \mathbb{N}} \qquad
    \frac{\Gamma \vdash n : \mathbb{N}}{\Gamma \vdash S(n) : \mathbb{N}} \qquad
    \cdots
\\]

On a tangential (but still very much related) note: I am setting myself some tertiary goals for the summer and the coming year. There's three key projects I want to work on:

1. A proof of strong normalisation for subtype universes in the [Coq proof assistant](https://coq.inria.fr/)
2. An introductory text/video series on type theory aimed at undergraduates
3. Finally sitting down and properly learning category theory

Let's break these goals down and see why I'm interested in them.

---

1. A proof of strong normalisation for subtype universes in the Coq proof assistant

As of writing this post, a paper I've written with my supervisor Zhaohui Luo has been accepted for publishing in the post-proceedings of TYPES22. _On the Metatheory of Subtype Universes_ generalises prior work on subtype universes and offers proofs for logical consistency, strong normalisation, decidability of type checking, etc. in a very brief 20 pages. But what's a paper on type theory without a computer-verified proof? 

I'm currently working out how write a proof in Coq of our work, and how to translate key ideas in our paper into something useful in a proof assistant. While the type theory our paper discusses isn't quite as powerful as the one Coq uses (and thus theoretically could have a complete computer-verifiable proof of strong normalisation and the like), this is also very much a question of what is sensible and feasible - especially as I haven't done work like this before. I'm hoping to start 'small' with a Coq proof of a much smaller theory - for example, one that doesn't contain dependent functions, dependent pairs, or inductive types -  in hopes that translating the proof from there into a 'larger system' will make for lighter work.

2. An introductory text/video series on type theory aimed at undergraduates

My initial exposure to type theory was during my undergraduate degree, when I first learned about proof assistants and started practicing with the [Lean proof assistant](https://leanprover.github.io/). As my curiosity grew and I wanted to find out how these systems worked, I discovered homotopy type theory and started reading from the [univalent foundations book](https://homotopytypetheory.org/book/).

3. Finally sitting down and properly learning category theory

When I 

---
---

[^1]: For those unfamiliar with the United Kingdom's system: PhD students will often not formally start on a degree which will award a doctorate. Instead, they will start on a masters by research degree (MPhil) and are later transferred onto a PhD degree after a year or two, once they have enough evidence to suggest they will be able to successfully finish a PhD.

[^2]: This website is built and maintained using [Jekyll](https://jekyllrb.com/). I'm using the wonderful [Chirpy theme](https://chirpy.cotes.page/) developed by Cotes Chung - I found the balance between its blog-first content and its adaptability for dedicated static content to be exactly what I needed. Plus it looks pretty.