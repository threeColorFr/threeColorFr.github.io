---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

![picture](/images/Myphoto.jpg)

{% for post in site.publications reversed %}
  {% include archive-single.html %}

  {% if post.cover_image %}
    <img src="{{ post.cover_image }}" alt="文章封面图片">
  {% endif %}
{% endfor %}
