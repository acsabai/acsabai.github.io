# {{ page.dir }}
aaaa
{{ page.dir }}
bbb


{% for file in site.static_files %}
	__{{file.path}}__
	{% if file.path contains {{ page.dir }} %}
		* [{{ file.path }}]({{ site.baseurl }}{{ file.path }})
	{% endif %}
{% endfor %}