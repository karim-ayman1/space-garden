---
layout: page
title: Home
id: home
permalink: /
banner_lock: true
banner: "https://images.unsplash.com/photo-1616355788928-edee67cca469?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1632&q=80"
---

# Welcome to my tiny blog

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 8px;">
karim ayman salah el den  loves to learn new things and share what I know with others. I'm a  <span style="font-weight: bold">crazy</span> programmer. I love to push the limits of what's possible with code. I love to find new and creative ways to use code to solve problems. And I love to share my discoveries with the world.
</p>

<strong>Recent Additions</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
