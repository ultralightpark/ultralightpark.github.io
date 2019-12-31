---
title: Home
layout: default
navigation_weight: 1
---
<ul>
  {% for post in site.posts %}
    <li>
      <div class= "post">
        {% if post.image %} <img src= "/content/{{ post.image }}.png"> {% endif %}
        <div class= "post-content">
          {{ post.content }}
          <div class = "post-meta">
            <div class = "post-nowplaying">
              {% if post.description %} <p>{{ post.description }}</p> {% endif %}
            </div>
            <div class = "post-permalink">
              #{{ post.title }} | <a href="{{ post.url }}">𝖕𝖊𝖗𝖒𝖆𝖑𝖎𝖓𝖐</a>
            </div>
          </div>
        </div>
       </div>
    </li>
  {% endfor %}
</ul>