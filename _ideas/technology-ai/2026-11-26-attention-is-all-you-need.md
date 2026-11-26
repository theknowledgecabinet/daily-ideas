---
layout: idea
title: Attention Is All You Need
date: 2026-11-26 08:13:40 +0000
description: The next time a chatbot answers you fluently, the machinery underneath it traces back to a 2017 bet on machine translation.
permalink: /technology-ai/2026-11-26-attention-is-all-you-need/
kind: article
kind_label: Article
icon: 📰
topic: Technology & AI
topic_slug: technology-ai
colour: '#2b6cb0'
source: arXiv
source_url: https://arxiv.org/abs/1706.03762
author: Ashish Vaswani and seven co-authors
published: '2017-06-12'
takeaways:
- The Transformer architecture throws out sequential memory processing entirely, letting every word consider every other word at once.
- 'The authors'' own numbers: record-setting translation quality at a small fraction of the usual training cost, thanks to full parallelism.'
- The mechanism behind modern large language models came from a machine translation paper, which helps explain why these systems are so fluent.
try_this: Read the paper's abstract on arXiv (about five minutes, one page), then read any paragraph you like out loud and ask, word by word, which earlier word each one is really paying attention to.
why: The next time a chatbot answers you fluently, the machinery underneath it traces back to a 2017 bet on machine translation.
audio:
  url: /assets/ideas/2026-11-26-attention-is-all-you-need/audio.mp3
  bytes: 926012
  seconds: 154
  length: 3 min
image:
  card:
    url: /assets/ideas/2026-11-26-attention-is-all-you-need/card.webp
    w: 400
    h: 301
  medium:
    url: /assets/ideas/2026-11-26-attention-is-all-you-need/medium.webp
    w: 800
    h: 602
  large:
    url: /assets/ideas/2026-11-26-attention-is-all-you-need/large.webp
    w: 1400
    h: 1054
  share:
    url: /assets/ideas/2026-11-26-attention-is-all-you-need/share.jpg
  color: '#33291f'
  alt: ''
  artist: Rembrandt
  licence: Public domain
  licence_url: null
  page: https://commons.wikimedia.org/wiki/File:Rembrandt_-_The_Anatomy_Lesson_of_Dr_Nicolaes_Tulp.jpg
prev:
  url: /philosophy/2026-11-25-happiness-is-what-you-do/
  title: Happiness is what you do
---
{% raw %}
In 2017, eight Google researchers published a paper called Attention Is All You Need. Machine translation systems at the time were built on sequential memory: recurrent networks that processed words one at a time, each passing the baton to the next. The paper's proposal was radical and simple. Toss the memory part away and build the whole model from attention alone, the same mechanism that had already been quietly used to connect the encoder and decoder in the best existing systems.

Attention is best thought of as a question each word asks of the others in a sentence: which of you matter? In 'the dog chased the cat because it was fast', it lands on dog rather than cat, and the model works out those weightings for every word at once, in one big matrix operation, instead of walking down the sentence step by step.

The results were all machine translation. On English-to-German, the model reached 28.4 BLEU, more than two points above the previous best, including ensembles. On English-to-French, 41.8 BLEU, a single-model record, after 3.5 days of training on eight GPUs, a small fraction of the cost of the competing systems. The authors also showed the architecture generalizing to English constituency parsing.

The reason it matters beyond translation is written in the abstract itself: the models are more parallelizable, and they train in significantly less time. Sequential networks had to wait for each word's turn; attention is a matrix operation, so a whole GPU farm can work on it at once. That property, scaled up, is what made large language models possible. The machinery inside most modern AI traces back to a 2017 bet on translation.
{% endraw %}
