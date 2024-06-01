---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: single
classes: wide

---


<div class="banner">
  <img src="{{ 'assets/images/banner.png' | relative_url }}" alt="">
  <div class="button-container">
    <a href="#research" class="button">Research</a>
    <a href="#publications" class="button">Publications</a>
    <a href="#contact" class="button">Contact</a>
  </div>
</div>

<section class="portfolio">
  <h2>Recent Posts</h2>
  <div class="posts">
    {% for post in site.posts limit:3 %}
    <div class="post">
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt }}</p>
      <a href="{{ post.url }}" class="read-more">Read more</a>
    </div>
    {% endfor %}
  </div>
</section>