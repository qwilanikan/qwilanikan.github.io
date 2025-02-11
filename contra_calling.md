---
layout: separate_page
permalink: /contra_calling/
title_1: Qwill Duvall - Contra Dance Caller
---
<img class="col one right profile-pic" src="/img/calling/calling_cropped.jpeg">

<br/>
Hello all! I am a contra dancer and caller from the midwest.  I began contra dancing in 2015 shortly after moving to Chicago.  A couple years later I began regularly traveling for dancing and I started calling in 2019.  I called regularly in the Chicago area during 2019 and the beginning of 2020, and I was just thinking about going on tour when the pandemic hit.  Since my work is now remote and dances have started back up, I am now on the road and touring! I've been at it since the beginning of 2023. I've called on both coasts, in the midwest and a smattering of other places!

I aim to be, friendly, clear and welcoming in my teaching and calling and to create programs that help to build the skill of dancers at each evening such that we can dance interesting and fun dances! I am excited to share some unusual dances and figures in my programs, and I have a particular soft spot for chains other than Robin's right hand chains! I have fun when I'm calling and I try to make dances fun for everyone!
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
  References available on request.
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
