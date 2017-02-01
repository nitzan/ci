---
layout: index
title: Assignments
category: assignments
permalink: /assignments/
---
<div class="wrapper index-wrapper">
	<ul class="index">
	    {% for post in site.assignments %}  
	    	<a href="{{post.url}}"> 
		        <li>
					{{ post.title }} {% if post.studio %}<sup>studio</sup>{% endif %}{% if post.lab %}<sup>lab</sup>{% endif %}<sup>{{ post.due }}</sup>
		        </li>
	        </a>
	    {% endfor %}
	</ul>
</div>