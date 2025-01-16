---
layout: default
---


<div class="home">

    <h2 class="page-heading">All Posts</h2>
  
 
      {% assign previous_year = null %}
      {% for post in site.posts %}
        {% assign current_year = post.date | date: "%Y" %}
        {% if previous_year and current_year != previous_year %}
          <hr style="width: 100%; margin-left: 0; border: none; border-top: 1.5px solid;">
        {% elsif previous_year %}
          <hr style="width: 200px; margin-left: 0; border: none; border-top: 0.6px dotted; border-spacing: 15px;">
        {% endif %}
			<h3><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
          	<time datetime="{{ post.date | date_to_xmlschema }}" class="post-meta by-line"> {{ post.date | date: "%-d %B %Y" }}  | <i>{{ post.author }}</i> </time> 
          	<p class="post-meta by-line">{{ post.description }}</p>
        {% assign previous_year = current_year %}
      {% endfor %}

  
</div>