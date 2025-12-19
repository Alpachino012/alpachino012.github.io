---
layout: default
title: Projects
permalink: /projects/
---

<h1>Projects</h1>
<p>Here are some of the projects I've worked on.</p>

<div style="margin-top: 30px;">
  {% for post in site.posts %}
    <div style="margin-bottom: 40px;">
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <span style="color: #888; font-size: 0.9rem;">{{ post.date | date: "%B %d, %Y" }}</span>
      <p>{{ post.excerpt }}</p>
      <a href="{{ post.url | relative_url }}" style="font-weight: bold; font-size: 0.9rem;">Read Project &rarr;</a>
    </div>
    <hr style="border: 0; border-top: 1px solid #eee;">
  {% endfor %}
</div>