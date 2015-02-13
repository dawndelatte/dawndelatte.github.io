---
layout: journal
title: journal
permalink: /journal/
---
<div class="home">
<div class="post_snippet">
<div class="post-list">
    {% for post in site.posts %}
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
    {% endfor %}
  </div>
  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
  </div>
</div>