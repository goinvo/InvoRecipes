---
layout: default
title: Home
---

{% assign collection = site.recipes | group_by: "category" %}
{% for group in collection %}
<div data-category="{{group.name}}">
<h2>{{group.name}}</h2>
<ul>
	{%for recipe in group.items%}
	<li><a href="{{recipe.url}}">{{recipe.title}}</a></li>
	{%endfor%}
</ul>

</div>
{%endfor%}
