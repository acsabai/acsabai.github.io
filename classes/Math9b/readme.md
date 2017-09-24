{% for file in site.static_files %}
{% if file.path contains page.dir %}
{% if file.path contains "/downloads/" %}
   - [{{ file.path | remove: page.dir }}]({{ site.baseurl }}{{ file.path }})
{% endif %}
{% endif %}
{% endfor %}