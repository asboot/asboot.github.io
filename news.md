---
layout: page
title: News
---

{% if site.categories.release %}
<span class="cat release">release</span>
<ul>
	{% for release in site.categories.release %}
		<li>
			{{ release.date | date_to_string }} &raquo; <a href="{{ release.url }}">{{ release.title }}</a>
		</li>
	{% endfor %}
</ul>
{% endif %}

{% if site.categories.update %}
<span class="cat update">update</span>
<ul>
	{% for update in site.categories.update %}
		<li>
			{{ update.date | date_to_string }} &raquo; <a href="{{ update.url }}">{{ update.title }}</a>
		</li>
	{% endfor %}
</ul>
{% endif %}

{% if site.categories.bug %}
<span class="cat bug">bug</span>
<ul>
	{% for bug in site.categories.bug %}
		<li>
			{{ bug.date | date_to_string }} &raquo; <a href="{{ bug.url }}">{{ bug.title }}</a>
		</li>
	{% endfor %}
</ul>
{% endif %}