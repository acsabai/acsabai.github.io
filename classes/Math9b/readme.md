{% for file in site.static_files %}
{% if file.path contains page.dir %}
   - [{{ file.path | remove: page.dir }}]({{ site.baseurl }}{{ file.path }})
{% endif %}
{% endfor %}