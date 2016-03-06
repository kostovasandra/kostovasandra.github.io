---
layout: image
title: Favourite groups
permalink: /groups
image: /image/nota.jpg
---
<br>
{% for group in site.data.groups %}
* **{{ group.name }}**
	{% for song in group.songs %}
	["{{ song.name }}"]({{ song.url }})
	{% endfor %}  
{% endfor %}

<br><br>

<footer>
 	<ul>
   		<li><a href="http://kostovasandra.github.io/">My Blog</a></li>
     	<li><a href="https://github.com/kostovasandra">Github</a></li>
	</ul>
</footer>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>
<script src="/js/bootstrap.min.js"></script>