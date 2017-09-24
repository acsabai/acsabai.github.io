#### This lecture ...

$$\sqrt{16} = 4$$

- [another page here](another.md)

#### Downloads:
{% for file in site.static_files %}
{% if file.path contains page.dir %}
{% if file.path contains "/downloads/" %}
   - [{{ file.path | remove: page.dir | remove: "downloads/" }}]({{ site.baseurl }}{{ file.path }})
{% endif %}
{% endif %}
{% endfor %}