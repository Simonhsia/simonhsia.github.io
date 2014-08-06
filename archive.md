---
layout: page
permalink: /archive/
title: ARCHIVE
---
<ul class="archive">
    {% for post in site.posts %}
      <li>
        <span class="archive_date">{{ post.date | date: "%Y-%m-%d" }}</span>&nbsp;&nbsp;&nbsp;
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </li>
    {% endfor %}
</ul>