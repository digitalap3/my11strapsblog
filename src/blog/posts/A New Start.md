---
creator: digitalap3
date: 2022-06-01
headerPic: /headers/default-post.jpg
summary: I have been bitten by the blog bug.  Again.  This iteration I am moving to the 11ty static site generator
pin: no
tags: ['musings', 'post', 'about']
slug: 2022/April/a-new-start.html
title: A New Start

---

I have been bitten by the blog bug.  Again.  This iteration I am moving to the [11ty static site generator](https://www.11ty.dev/), which is built with nodejs.  Previously I was hacking my absolute most favorite piece of software [tiddlywiki](https://tiddlywiki.com/) to use as an SSG and although I did absolutely enjoy the project, it just feels like reinventing the wheel in a far inferior form.  I will still be using tiddlywiki to write drafts and I have modified it to provide output formatted for 11ty which will be the subject of my initial posts.  All of the tiddlywiki code still resides on my [github page](https://github.com/digitalap3/tiddlywikistaticsitegen) if someone by some bizarre twist comes upon this obscure part of the webs.

In addition to the quite lofty goals I have set for myself in [My Intent for This Blog](/blog/2022/April/my-intent-for-this-blog.html) I will be posting lots of, actually probably more of, wonderfully mundane family pictures like this:

{% set imgUrl = '/2022/April/OGKidsatthetable.jpg' %}
{% set size = "80%" %}
{% set imgCaption = "I have no idea what I'm saying but it must be amazing" %}

  {% include "partials/figure-center.html" %}
