---
layout: page
title: Projects
permalink: /projects/
---
<div class='gallery-nav'>
  <div class="controls">
        <ul style="margin-left:0">
          <li>
            <button type="button" class="control" data-filter="all">Show All</button>
          </li>
          <li>
            <button type="button" class="control" data-filter=".big">Big Games</button>
          </li>
          <li>
            <button type="button" class="control" data-filter=".small">Small Games</button>
          </li>
          <li>
            <button type="button" class="control" data-filter=".if">Interactive Fiction</button>
          </li>
          <li>
            <button type="button" class="control" data-filter=".physical">Physical Installations</button>
          </li>
        </ul>
    </div>
</div>

<div class="container">
{% for project in site.projects %}
        {% if project.category == 'big game' %}
            <div class="mix big">
              <a href='{{ site.baseurl }}{{ project.url }}'>
                <img class="thumbnail" alt="" src="{{ project.img }}" />
                <div class="overlay">
                  <div class='thumb-info'>
                    <h4>{{ project.title }}</h4>
                    </br>
                    <p>{{ project.description }}</p>
                  </div>
                </div>
              </a>
            </div>
        {% endif %}
        {% if project.category == 'small game' %}
            <div class="mix small">
              <a href='{{ site.baseurl }}{{ project.url }}'>
                <img class="thumbnail" alt="" src="{{ project.img }}" />
                <div class="overlay">
                  <div class='thumb-info'>
                    <h4>{{ project.title }}</h4>
                    </br>
                    <p>{{ project.description }}</p>
                  </div>
                </div>
              </a>
            </div>
        {% endif %}
        {% if project.category == 'interactive fiction' %}
            <div class="mix if">
              <a href='{{ site.baseurl }}{{ project.url }}'>
                <img class="thumbnail" alt="" src="{{ project.img }}" />
                <div class="overlay">
                  <div class='thumb-info'>
                    <h4>{{ project.title }}</h4>
                    </br>
                    <p>{{ project.description }}</p>
                  </div>
                </div>
              </a>
            </div>
        {% endif %}
        {% if project.category == 'physical' %}
            <div class="mix physical">
              <a href='{{ site.baseurl }}{{ project.url }}'>
                <img class="thumbnail" alt="" src="{{ project.img }}" />
                <div class="overlay">
                  <div class='thumb-info'>
                    <h4>{{ project.title }}</h4>
                    </br>
                    <p>{{ project.description }}</p>
                  </div>
                </div>
              </a>
            </div>
        {% endif %}
      {% endfor %}

  <div class="gap"></div>
  <div class="gap"></div>
  <div class="gap"></div>
</div>

<script>
          var container1 = document.querySelector('.container');
          var mixer = mixitup(container1, {
            animation: {
              enable: true
            }
          });
      </script>
