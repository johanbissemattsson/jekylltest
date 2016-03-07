<ul>
{% assign sorted_pages = site.pages | sort:"name" %}
{% for node in sorted_pages %}
  <li><a href="{{node.permalink:slug}}">{{node.title}}</a></li>
{% endfor %}
</ul>
