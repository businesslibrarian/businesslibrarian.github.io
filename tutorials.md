---
layout: default
# Blog | Simple Jekyll
header: Tutorials
summary: A list of tutorials for business resources.
link: /tutorials/
---

{% for post in site.posts %}
  <section>
  <p><a href="{{ post.url }}">{{ post.title }}</a><br>
  <br>
  {{ post.summary }}<br>
  <br>
  {{ post.date | date_to_string }}</p>
  </section>
{% endfor %}