---
templateKey: blog-post
title: Many-shot jailbreaking
date: 2024-04-03T12:07
description: > 
  New Anthropic research paper: Many-shot jailbreaking.


  We study a long-context jailbreaking technique that is effective on most large language models, including those developed by Anthropic and many of our peers.
featuredpost: true
featuredimage: https://pbs.twimg.com/media/GKLM9f_WIAAZvLE?format=jpg&name=medium
---
*Original Article:*

<https://www.anthropic.com/research/many-shot-jailbreaking>



We investigated a “jailbreaking” technique — a method that can be used to evade the safety guardrails put in place by the developers of large language models (LLMs). The technique, which we call “many-shot jailbreaking”, is effective on Anthropic’s own models, as well as those produced by other AI companies. We briefed other AI developers about this vulnerability in advance, and have implemented mitigations on our systems.

The technique takes advantage of a feature of LLMs that has grown dramatically in the last year: the context window. At the start of 2023, the context window—the amount of information that an LLM can process as its input—was around the size of a long essay (~4,000 tokens). Some models now have context windows that are hundreds of times larger — the size of several long novels (1,000,000 tokens or more).

The ability to input increasingly-large amounts of information has obvious advantages for LLM users, but it also comes with risks: vulnerabilities to jailbreaks that exploit the longer context window.

One of these, which we describe in our new paper, is many-shot jailbreaking. By including large amounts of text in a specific configuration, this technique can force LLMs to produce potentially harmful responses, despite their being trained not to do so.

Below, we’ll describe the results from our research on this jailbreaking technique — as well as our attempts to prevent it. The jailbreak is disarmingly simple, yet scales surprisingly well to longer context windows.

Continue Reading <https://www.anthropic.com/research/many-shot-jailbreaking>
