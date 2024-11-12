---
layout: default
# Blog | Simple Jekyll
header: Tutorials
summary: A list of tutorials for business resources.
link: /tutorials/
---

{% for post in site.posts %}
  <p><a href="{{ post.url }}">{{ post.title }}</a><br>
  {{ post.description }}<br>
  {{ post.date | date_to_string }}</p>
{% endfor %}