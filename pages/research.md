---
title: "Quantitative Criminology Research Cluster"
layout: splash
permalink: /pages/research/
header:
  overlay_color: "#000"
  overlay_filter: "0.6"
  overlay_image: /assets/images/splash/London_gangs_1.png
  actions:
    - label: "Members"
      url: "/pages/members/"
    - label: "Our Research"
      url: "/pages/research/"
    - label: "Events & Webinars"
      url: "/pages/events/"
    - label: "Our Partners"
      url: "/pages/partners/"
---

<h1>Our Projects</h1>
<div class="posts-grid">
  {% for post in site.posts %}
    {% if post.categories contains "research" %}
      <div class="post-item">
        <a href="{{ post.url | relative_url }}">
          {% if post.image %}
            <img src="{{ post.image | relative_url }}" alt="{{ post.title }}" class="post-image">
          {% endif %}
          <h2>{{ post.title }}</h2>
          <p>{{ post.excerpt }}</p>
        </a>
      </div>
    {% endif %}
  {% endfor %}
</div>