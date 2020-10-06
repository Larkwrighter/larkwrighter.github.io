---
layout: page
title: My Work
permalink: /projects/
---

<div class="container">
    
    <div class="grid-container">

    {% for post in site.posts %}

        <div class="grid-item">
            <a href='{{ site.baseurl }}{{ post.url | prepend: site.baseurl }}'>
                <img class="thumbnail" alt="" src="{{ post.image }}" />
                <div class="overlay">
                  <div class="thumb-info">
                    <h2 class="thumb-title">{{ post.title }}</h2>
                    <!--<p>{{ post.thumbnail }}</p>-->
                  </div>
                </div>
            </a>  
        </div>

    {% endfor %}

    </div>

</div>