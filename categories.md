---
layout: page
title: All Post
description: All Post Materi FD.
header: All Post
---


<!-- 
*********************************************
FOR FD 2022  
*********************************************
-->

<!-- 
*********************************************
EXPERIMENT 2 : ??
*********************************************
-->
<!-- { if post.title == "Cybercrime Forensik Digital -" } -->
<ul>
    {% for post in site.posts %}
        
        {% if post.title contains "Kuliah FORENSIK DIGITAL" or post.title contains "Cybercrime Forensik Digital  - 19000" or post.title contains "Hasil Tugas Pertemuan" %}
            <li>
                <!-- <a href="{{ post.url | prepend: site.url }}" target="_blank">{{ post.date | date: "%-d %B %Y" }} - {{ post.title }} [ {{ post.author }} ] </a> -->
                <a href="{{ site.url }}{{ site.baseurl }}{{ post.url}}" target="_blank">{{ post.date | date: "%-d %B %Y" }} - {{ post.title }} [ {{ post.author }} ] </a> 
            </li>
        {% endif %}

    {% endfor %}
</ul>


<!-- 
    ***

    <ul>
        <li><a href="#">Site URL : {{ site.url }}</a></li>
        <li><a href="#">Site BaseURL : {{ site.baseurl }}</a></li>
        <li><a href="{{ site.url }}{{ site.baseurl }}">SiteURL SiteBaseURL : {{ site.url }}{{ site.baseurl }}</a></li>
        <li><a href="#">Title URL : {{ title.url }}</a></li>
    </ul>
 -->


***
By: Ikhwan@fedora37.linux