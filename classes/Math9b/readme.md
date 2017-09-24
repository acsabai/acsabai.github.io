# {{ page.dir }}

aaaa

{{ page.dir }}

bbb

{{ page.path }}

{% for file in site.static_files %}
	* 11: {{file.path}}
	{% if file.path contains {{ page.dir }} %}
		* [{{ file.path }}]({{ site.baseurl }}{{ file.path }})
	{% endif %}
{% endfor %}