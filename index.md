---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
title: 
---
{% for post in site.posts %}
  <div id="post-short">
    <a href="{{site.url}}{{site.baseurl}}{{post.url}}">
      <h3>{{post.title}}</h3>
    </a>
    <i>Опубликовано {{ post.date | date: "%d.%m.%Y" }}</i>
    <p>
      {% if post.excerpt %}
        {{ post.excerpt }}
        <a href="{{site.url}}{{site.baseurl}}{{post.url}}">
          <p><b>Слушать и читать"</b></p>
        </a>
      {% else %}
        {{ post.content }}
        <a href="{{site.url}}{{site.baseurl}}{{post.url}}">
          <p><b>>> Слушать и читать</b></p><br>
        </a>
      {% endif %}
    </p>
  </div>
{% endfor %}
