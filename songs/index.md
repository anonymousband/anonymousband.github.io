---
layout: page
title: Our Music
permalink: /songs/
---
We are making lots of music at the moment. Check out this post:
[Latest Songs!]({{ site.baseurl }}{% post_url 2017-01-29-latest-songs %})

{% for post in site.categories.songs %}
    <a href="{{post.url}}">{{ post.title }}</a>
{% endfor %}

{% for category in site.categories %}
  <li><a name="{{ category | first }}">{{ category | first }}</a>
    <ul>
    {% for posts in category %}
      {% for post in posts %}
        <li><a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
    {% endfor %}
    </ul>
  </li>
{% endfor %}
