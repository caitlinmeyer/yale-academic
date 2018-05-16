---
layout: page
title: Blog
---

<ul id="posts">
	  <li class="post">
	  	<h2><a href="{% if site.baseurl == "/" %}{{ post.url }}{% else %}{{ post.url | prepend: site.baseurl }}{% endif %}">{%if post.header %}{{ post.header }}{% else %}{{ post.title }}{% endif %}</a></h2>
      <time datetime="{{ post.date | date_to_xmlschema }}" class="by-line"> <i>{{ post.date | date_to_string }}</i> </time>
	  </li>
</ul>
