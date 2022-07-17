---
layout: page
permalink: /categorias/
title: Explorar todas las categorías
background: '/img/bg-about.jpg'
---


<div id="archives">
{% for category in site.category %}
  <div class="archive-group">
    {% capture category_name %}{{ category.name }}{% endcapture %}
    {% capture category_title %}{{ category.title }}{% endcapture %}
    
    <div id="#{{ category_name | slugize }}"></div>
    <p></p>

    <a href="{{site.baseurl}}/category/{{ category_name | uri_escape }}.html"><h3 class="category-head">{{ category_title }}</h3>
    </a>
    {% for post in site.categories[category_name] %}
    <article class="archive-item">
      <li>{{ post.date | date: '%d/%m/%Y' }}:
        <a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a>
      </li>
    </article>
    {% endfor %}
  </div>
{% endfor %}
</div>
