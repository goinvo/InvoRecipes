---
layout: default
title: Home
---

{% assign collection = site.recipes | group_by: "category" %}
{% for group in collection %}
<h2>{{group.name}}</h2>
	{%for recipe in group.items%}
<a href="{{recipe.url}}">{{recipe.title}}</a>
{%endfor%}
{%endfor%}
