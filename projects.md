---
layout: page
title: Projects
permalink: /projects/
---

<div class="categorybar">
<h3>Games</h3>
</div>

{% for project in site.projects %}
{% if project.category == 'game' %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h4>{{ project.title }}</h4>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
    <h4 style="padding-top:5px;text-align:left">{{ project.title }} ({{project.year}})</h4>
</div>
{% else %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h4>{{ project.title }}</h4>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
    <h4 style="padding-top:5px;padding-bottom:50px;margin">{{ project.title }} ({{project.year}})</h4>
</div>
{% endif %}


{% endif %}

{% endfor %}

<div class="categorybar" style="padding-top: 32px">
<h3>Interactive Fiction</h3>
</div>

{% for project in site.projects %}

{% if project.category == 'interactive fiction' %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h4>{{ project.title }}</h4>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
    <h4 style="padding-top:5px">{{ project.title }} ({{project.year}})</h4>
</div>
{% else %}
<div class="project ">
    <div class="thumbnail">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h4>{{ project.title }}</h4>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
    <h4 style="padding-top:5px">{{ project.title }} ({{project.year}})</h4>
</div>
{% endif %}


{% endif %}

{% endfor %}

<!--<div class="categorybar" style="padding-top: 32px">
<h3>Other</h3>
</div>

{% for project in site.projects %}

{% if project.category == 'other' %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h4>{{ project.title }}</h4>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}
<div class="project ">
    <div class="thumbnail">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% endif %}


{% endif %}

{% endfor %}-->