---
layout: separate_page
permalink: /contra_calling/
title_1: Qwill Duvall - Contra Dance Caller
---
<img class="col one right profile-pic" src="/img/calling/calling_cropped.jpeg">

<br/>
Qwill discovered contra dancing when they moved to Chicago in 2015, drawn by its welcoming, intergenerational community, culture of dancing both roles, and the joy of connecting with everyone in the room. They were inspired to start calling in 2019. Qwill has been touring nationally since 2023 — primarily along the East Coast, but also bringing their dynamic calling to the Midwest and the West Coast. Along the way, they’ve shared the stage with beloved bands such as Hot Seat, Chimney Swift, Northwoods, Cojiro and Daybreak Trio.

Qwill brings an upbeat, playful energy to every dance, making the experience both welcoming and exciting. With clear, relaxed teaching and an eye for the skill level in the room, they keep dancers engaged — whether with creative choreography, unusual figures, or simply a well-chosen, satisfying dance. Expect a fun, inclusive atmosphere where beginners feel supported, experienced dancers stay intrigued, and everyone leaves smiling.
<!--<a href="http://fortawesome.github.io/Font-Awesome/" target="blank">Font Awesome icons</a>-->

<br/>
<hr/>
<br/>
<span class="contacticon center">
	<a href="mailto:qwill.duvall@gmail.com"><i class="fa fa-envelope-square"></i></a>
	<a href="http://facebook.com/QwillDuvallContraDanceCaller" target="_blank"><i class="fa fa-facebook-square"></i></a>
</span>

<div class="col three caption">
	Shoot me an email if you'd like to book me for a gig!
  <br/>
  References available upon request.
</div>

<br/>
<hr/>
<br/>


{% for project in site.contra_calling reversed %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail display-title">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.year }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project">
    <div class="thumbnail display-title">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.year }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %}
