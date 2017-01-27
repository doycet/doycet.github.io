---
layout: default
---

<div class="well">
{% for category in site.categories %}
<h1>{{ category | first }}</h1>
    {% for posts in category %}
      {% for post in posts %}
      {% if post.url %}  

* <a href="{{ post.url }}">{{ post.title }}</a><br>  

    {% endif %}
      {% endfor %}
    {% endfor %}
{% endfor %}
</div>


