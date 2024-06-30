---
title: "Quantitative Criminology Research Cluster"
layout: splash
permalink: /pages/events/
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

<div class="events-page">
  <aside class="sidebar">
    <h2>Archive</h2>
    <ul>
      {% assign years = "" %}
      {% for post in site.posts %}
        {% if post.categories contains "events" or post.categories contains "webinar" or post.categories contains "interview" %}
          {% assign year = post.date | date: "%Y" %}
          {% unless years contains year %}
            {% assign years = years | append: year | append: "," %}
            <li><a href="#{{ year }}">{{ year }}</a></li>
          {% endunless %}
        {% endif %}
      {% endfor %}
    </ul>
    <h2>Categories</h2>
    <ul>
      {% assign categories = site.posts | map: 'categories' | uniq %}
      {% for category in categories %}
        {% if category contains "events" or category contains "webinar" or category contains "interview" %}
          <li><a href="#{{ category }}">{{ category | capitalize }}</a></li>
        {% endif %}
      {% endfor %}
    </ul>
  </aside>

  <div class="posts-events-content">
    <h1>Events and Webinars</h1>
    <div class="posts-events-list">
      {% assign current_date = "" %}
      {% for post in site.posts %}
        {% if post.categories contains "events" or post.categories contains "webinar" or post.categories contains "interview" %}
          {% assign post_date = post.date | date: "%B %Y" %}
          {% if post_date != current_date %}
            {% assign current_date = post_date %}
            <h2 class="post-events-date">{{ current_date }}</h2>
          {% endif %}
          <div class="post-events-item">
            <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
            {% if post.image %}
              <img src="{{ post.image | relative_url }}" alt="{{ post.title }}" class="post-events-image">
            {% endif %}
            <p>{{ post.excerpt }}</p>
          </div>
        {% endif %}
      {% endfor %}
    </div>
  </div>
</div>

