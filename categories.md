---
layout: page
title: All Post
description: This page displays all posts.
header: All Post
---


<!-- ### List Post V1 -->

<!-- 
{% for post in site.posts %}
    {% if post.categories contains 'postcategory' %}
    <h1>Do nothing</h1>
    {% else %}
    <h2>{{ post.title }}</h2>
    {% endif %}
{% endfor %} 
-->

<ul>
{% for post in site.posts %}
        <li><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }} [ {{ post.author }} ] </a></li>
    <!-- [{{ post.title }}]({{ post.title }}){:target="_blank"} -->

{% endfor %}
</ul>

***
By: Ikhwan@fedora37.linux