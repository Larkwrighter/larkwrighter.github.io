---
layout: page
title: Blog
permalink: /blog/
---

<ul class="post-list">
    {% for post in site.blog reversed %}
      <li>
        <h2 style="padding-bottom: 10px;"><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
        <!--<div class="blog-img">
        {% if post.img %}
        <img src="{{ post.img }}"/>
        {% endif %}
        </div>-->
        <br />
        <p class="post-meta">Posted {{ post.date | date: '%B %-d, %Y' }} in {{ post.category }}</p>
        <br />
        <p>{{ post.excerpt }}</p>
        <p><a style="" href="{{ post.url | prepend: site.baseurl }}">Read More...</a></p>
        <hr/>
      </li>
    {% endfor %}
</ul>