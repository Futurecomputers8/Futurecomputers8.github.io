---
layout: default
title: Future Computers 2030–2040
description: "Computers 2030–2040: quantum revolution, brain-computer interfaces, DNA storage, ambient computing, zero screens, and the end of traditional PCs."
---

<div class="posts-grid">
  {% assign sorted_posts = site.posts | reverse %}
  {% for post in sorted_posts %}
    {% assign first_image = post.content | split:'src="' | slice:1 | first | split:'"' | first %}

    <article class="post-card">
      <a href="{{ post.url }}">
        <div class="post-thumb-wrapper">
          <img src="{{ first_image }}" alt="{{ post.title }}" class="post-thumb">
        </div>
        <div class="post-info">
          <h2>{{ post.title | split: ". " | last }}</h2>
          <p class="post-desc">{{ post.description }}</p>
          <span class="read-more">Read chapter</span>
        </div>
      </a>
    </article>
  {% endfor %}
</div>

<div class="made-with">
  <p>All images • Full offline • No tracking • Built December 2025</p>
</div>
