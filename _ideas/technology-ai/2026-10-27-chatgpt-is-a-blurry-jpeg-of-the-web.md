---
layout: idea
title: ChatGPT is a blurry JPEG of the web
date: 2026-10-27 08:34:56 +0000
description: The blur is invisible until you put the original next to it, and most of our AI answers arrive without one.
permalink: /technology-ai/2026-10-27-chatgpt-is-a-blurry-jpeg-of-the-web/
kind: article
kind_label: Article
icon: 📰
topic: Technology & AI
topic_slug: technology-ai
colour: '#2b6cb0'
source: The New Yorker
source_url: https://www.newyorker.com/tech/annals-of-technology/chatgpt-is-a-blurry-jpeg-of-the-web
author: Ted Chiang
published: '2023-02-09'
takeaways:
- A photocopier once printed three different room sizes as the same number. The copies were readable, and that is exactly what made them dangerous.
- If a language model is a lossy compression of the web's text, you will never get the exact words back. Hallucinations are the artifacts, and the only dependable check is the original.
- 'Chiang''s closing question: when you still have the original, how much use is the blurry JPEG?'
caveats: This is a science fiction writer's analogy, not a formal account of how large language models work. The compression picture is a lens for understanding hallucinations and style imitation, not a technical property of ChatGPT, and the essay is a 2023 snapshot of that particular system.
try_this: 'Next time a chatbot hands you a confident fact, figure or quote, spend ten minutes treating it as a photocopy: open the original source, check the exact wording, and note where the copy drifted.'
why: The blur is invisible until you put the original next to it, and most of our AI answers arrive without one.
audio:
  url: /assets/ideas/2026-10-27-chatgpt-is-a-blurry-jpeg-of-the-web/audio.mp3
  bytes: 1298972
  seconds: 216
  length: 4 min
image:
  card:
    url: /assets/ideas/2026-10-27-chatgpt-is-a-blurry-jpeg-of-the-web/card.webp
    w: 400
    h: 600
  medium:
    url: /assets/ideas/2026-10-27-chatgpt-is-a-blurry-jpeg-of-the-web/medium.webp
    w: 800
    h: 1200
  large:
    url: /assets/ideas/2026-10-27-chatgpt-is-a-blurry-jpeg-of-the-web/large.webp
    w: 1400
    h: 2100
  share:
    url: /assets/ideas/2026-10-27-chatgpt-is-a-blurry-jpeg-of-the-web/share.jpg
  color: '#55443c'
  alt: Ted Chiang , American science fiction author. Taken at 'Estudio en escarlata' library, Madrid, Spain, 24/02/2011.
  artist: Arturo Villarrubia
  licence: CC BY-SA 2.0
  licence_url: https://creativecommons.org/licenses/by-sa/2.0
  page: https://commons.wikimedia.org/wiki/File:Chiang,_Ted_(Portrait_by_Arturo_Villarrubia).jpg
prev:
  url: /philosophy/2026-10-26-choosing-your-attitude-frankl-s-last-freedom/
  title: 'Choosing your attitude: Frankl''s last freedom'
---
{% raw %}
In 2013, workers at a German construction company noticed something odd about their office Xerox copier. When they copied a house floor plan, the area label on every one of the three rooms came out as 14.13 square metres. The rooms were actually 14.13, 21.11 and 17.42. The computer scientist David Kriesel traced it to the machine's lossy compression format, JBIG 2, which looks for regions similar enough to store once and reuse. The three labels were similar enough. Xerox shipped a patch in 2014.

What made the incident dangerous was how readable the result was. The numbers came out clean, and clean numbers invite trust. A copy that is obviously blurry gets checked against the original. This one did not.

Ted Chiang, the science fiction writer, takes that incident in a 2023 essay as a way to think about ChatGPT. His thought experiment: imagine you are about to lose access to the internet forever and must store all of the web's text on a server with one per cent of the space you would need. You cannot store it verbatim, so you write a lossy algorithm that finds the statistical regularities in the text and keeps only those, at a hundred to one compression ratio. Now you can no longer look anything up by exact quote, because the original words are not stored. So you add an interface that answers questions in fresh words, conveying the gist of what it holds.

That, Chiang says, is what ChatGPT amounts to: a blurry JPEG of all the text on the web. It retains much of the information, but you will never get the exact words back, only an approximation. In this picture, hallucinations are compression artifacts. They are plausible text built from patterns in the data, wrong in the same way the photocopier's 14.13 was wrong, and the only real check is comparing them against the originals. Style imitation works by interpolation, estimating what goes between two known points, which is why a request for a lost sock described in the style of the Declaration of Independence yields a plausible sentence nobody would actually have written. Chiang notes that people treated this as a game, a blur tool for paragraphs instead of photos.

His closing question is the one to carry away. When you still have the original, how much use is a blurry JPEG? The answer depends on what you are doing. A summary of a long article is fine. An answer you plan to rely on is a photocopy, and it deserves to be checked.
{% endraw %}
