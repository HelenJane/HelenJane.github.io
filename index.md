---
layout: default
title: my first Blog
---

<h2>{{ page.title }}</h2>

<p>latest page </p>

<ul>

{% for post in site.posts %}

<li>{{ post.date | date_to_string }} <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>

{% endfor %}
</ul>