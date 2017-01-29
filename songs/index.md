---
layout: page
title: Our Music
permalink: /songs/
---
We are making lots of music at the moment. Check out this post:
[Latest Songs!]({{ site.baseurl }}{% post_url 2017-01-29-latest-songs %})

{% for post in site.categories.songs %}
<ul>
    <li><a href="{{post.url}}">{{ post.title }}</a></li>
</ul>
{% endfor %}
