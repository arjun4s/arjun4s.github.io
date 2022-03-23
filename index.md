---
layout: page2
title: Halo, Dunia!
tagline: 
---
{% include JB/setup %}
## Selamat Datang
Terima kasih atas kunjungan kamu di Kodeloka.

## Arsip Posting
<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## Permainan Favorit
<ul>
  <li><a href="https://arjun4s.github.io/sow98/programs/js-solitaire/index.html">Solitaire</a></li>
  <li><a href="https://arjun4s.github.io/sow98/programs/minesweeper/index.html">Minesweeper</a></li>
  <li><a href="https://arjun4s.github.io/sow98/programs/pinball/space-cadet.html">Pinball</a></li>
</ul>
