---
layout: index
title: Lectures
category: lectures
permalink: /lectures/
---
<div class="wrapper index-wrapper">
	<ul class="index">
	    {% for post in site.lectures %}  
	    	<a href="{{post.url}}"> 
		        <li>
					{{ post.title }} {% if post.studio %}<sup>studio</sup>{% endif %}{% if post.lab %}<sup>lab</sup>{% endif %}<sup>{{ post.due }}</sup>
					
		        </li>
	        </a>
	    {% endfor %}
	</ul>
</div>