# {{ page.dir }}

aaaa

{{ page.dir }}

bbb

{{ page.path }}

{% for file in site.static_files %}
	* [{{ file.path }}]({{ site.baseurl }}{{ file.path }})
{% endfor %}

{% for file in site.static_files %}
	{% if file.path contains {{ page.path }} %}
		* [{{ file.path }}]({{ site.baseurl }}{{ file.path }})
	{% endif %}
{% endfor %}