---
layout: page
title: Projects
permalink: /projects/
---

# My LLM-Assisted Projects

Projects with the assistance of Large Language Models.

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <h2>
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      </h2>
      <p>{{ post.date | date: "%B %d, %Y" }}</p>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

{% if site.posts.size == 0 %}
  <p>No projects have been added yet. Check back soon!</p>
{% endif %}
