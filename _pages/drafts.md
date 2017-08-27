---
layout: default
title: Drafts
permalink: /pages/drafts/
---
# Draft Posts

{% for post in site.posts reversed %}
{% if post.status == "draft" %}
  <p class="toc">{{ post.date | date_to_string }} &raquo; <a href="{{post.url | prepend:site.baseurl}}">{{ post.title}}</a></p>
  {% endif %}
  {% endfor %}
  <p></p>
