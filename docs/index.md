---
title: Documentation
layout: blog
---

[Papers](/docs/papers/)
------

{% for post in site.categories.papers limit:3 %}
<article class="pub paper">
  <span class="title"><a href="{{ post.url }}">{{ post.title | xml_escape }}</a></span>
  {% if post.uri %}
  <span class="uri">[<a href="{{ post.uri }}">link</a>]</span>
  {% endif %}

  {% if post.pdf %}
  <span class="pdf">[<a href="{{ post.pdf }}">pdf</a>]</span>
  {% endif %}

  {% if post.slides %}
  <span class="slides">[<a href="{{ post.slides }}">slides</a>]</span>
  {% endif %}

  {% if post.video %}
  <span class="video">[<a href="{{ post.video }}">video</a>]</span>
  {% endif %}

  <br />
  <span class="authors">{{ post.authors | xml_escape }}</span>
  <span class="venue">{{ post.venue | xml_escape }}</span>
  <span class="date">{{ post.date | date_to_long_string }}</span>

</article>
{% endfor %}

[Talks](/docs/talks/)
-----

{% for post in site.categories.talks limit:3 %}
<article class="pub talk">
  <span class="title"><a href="{{ post.url }}">{{ post.title | xml_escape }}</a></span>
  {% if post.uri %}
  <span class="uri">[<a href="{{ post.uri }}">link</a>]</span>
  {% endif %}

  {% if post.pdf %}
  <span class="pdf">[<a href="{{ post.pdf }}">pdf</a>]</span>
  {% endif %}

  {% if post.slides %}
  <span class="slides">[<a href="{{ post.slides }}">slides</a>]</span>
  {% endif %}

  {% if post.video %}
  <span class="video">[<a href="{{ post.video }}">video</a>]</span>
  {% endif %}

  <br />
  <span class="authors">{{ post.authors | xml_escape }}</span>
  <span class="venue">{{ post.venue | xml_escape }}</span>
  <span class="date">{{ post.date | date_to_long_string }}</span>

</article>
{% endfor %}