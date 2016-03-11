---
layout: image
title: Favourite groups
permalink: /groups
image: /image/nota.jpg
position: 800px 180px
size: 400px 400px
description: "Groups"
---

<br>
{% for group in site.data.groups %}
* **{{ group.name }}**
	{% for song in group.songs %}
	["{{ song.name }}"]({{ song.url }})
	{% endfor %}  
{% endfor %}


