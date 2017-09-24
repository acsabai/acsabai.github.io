
{% for file in site.static_files %}
  {% if file.path  contains page.dir %}
    * [{{ file.path }}]({{ site.baseurl }}{{ file.path }})
  {% endif %}
{% endfor %}