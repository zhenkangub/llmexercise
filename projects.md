---
layout: page
title: Projects
permalink: /projects/
---

# My LLM-Assisted Projects

This page showcases my journey of learning through building small, focused projects with the assistance of Large Language Models.

<div class="projects-list">
  {% for post in site.posts %}
    <div class="project-item">
      <h2>
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      </h2>
      <p class="project-date">{{ post.date | date: "%B %d, %Y" }}</p>
      {{ post.excerpt }}
      <div class="project-links">
        <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read more</a>
        {% if post.github_repo %}
          <a href="{{ post.github_repo }}" class="github-link" target="_blank">GitHub</a>
        {% endif %}
      </div>
    </div>
  {% endfor %}
</div>