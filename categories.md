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
                <a href="{{ post.url | prepend: site.baseurl }}">{{ post.date | date: "%-d %B %Y" }} - {{ post.title }} [ {{ post.author }} ] </a>
            </li>
        {% endif %}

    {% endfor %}
</ul>





***
By: Ikhwan@fedora37.linux