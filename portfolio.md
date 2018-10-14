---

layout: page

permalink: /portfolio/

title: portfolio
---



Here you can find some of the projects I've worked on and cool things I've done, whether they've been for class, an internship, a competition, or just for fun.

<br/>

This page is under maintenance.

<br/>

{% for project in site.portfolio %}

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

            <h1>{{ project.title }}</h1>

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

{% endfor %}
