---
layout: default
title: Research Group - Priya L. Donti
---

## Research Group

<!-- {% for grp in site.data.people %}
<h3 id="{{grp.anchor}}">{{grp.group}}</h3>
<div class="person__list">
{% for p in grp.members %}
{% if p.website_url %}
<a class="person__item" href="{{p.website_url}}" target="_blank">
{% else %}
<div class="person__item">
{% endif %}
<div class="person__pic-wrapper">
<img class="person__pic" src="{{p.image_url}}">
</div>
<div class="person__info">
<div class="person__name">{{p.name}}</div>
<div class="person__affil">{{p.affiliation}}</div>
{% if p.roles %}
<hr/>
<div class="person__role">
{% for role in p.roles %}
<span>{{role}}</span>
{% endfor %}
</div>
{% endif %}
</div>
{% if p.website_url %}
</a>
{% else %}
</div>
{% endif %}
{% endfor %}
</div>
{% endfor %} -->

{% for grp in site.data.people %}
<h3 id="{{grp.anchor}}">{{grp.group}}</h3>
<div class="member__list">

{% for p in grp.members %}

{% if p.website_url %}
<a class="member" href="{{p.website_url}}" target="_blank">
{% else %}
<div class="member">
{% endif %}

{% if p.image_url %}
<img src="{{p.image_url}}">
{% else %}
<img src="/img/group/default.png">
{% endif %}

<name>{{p.name}}</name><br><member_type>({{p.type}})</member_type>


{% if p.website_url %}
</a>
{% else %}
</div>
{% endif %}
{% endfor %}

</div>
{% endfor %}