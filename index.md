---
title: Home
layout: default
navigation_weight: 1
---
<ul>
  {% for post in site.posts %}
    <li>
      <div class= "post">
        <div class = "post-permalink">
          <a href="{{ post.url }}">#{{ post.title }}</a>
        </div>
        <div class= "post-content">
          {{ post.content }}
        </div>
       </div>
    </li>
  {% endfor %}
</ul>