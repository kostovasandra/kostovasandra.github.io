---
layout: image
title: Favourite singers
permalink: /singers
image: /image/nota.jpg
position: 800px 180px
size: 400px 400px
---

<br>
{% for singer in site.data.singers %}
* **{{ singer.name }}**
	{% for song in singer.songs %}
	["{{ song.name }}"]({{ song.url }})
	{% endfor %}  
{% endfor %}


