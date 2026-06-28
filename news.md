---
title: News
permalink: /news/
hide_header: true
compact_page: true
---

<div class="news-archive">
  {% for post in site.posts %}
  {% assign current_year = post.date | date: "%Y" %}
  {% if current_year != previous_year %}
    {% unless forloop.first %}</div>{% endunless %}
    <div class="archive-year">
      <h2>{{ current_year }}</h2>
  {% endif %}
      <a class="news-row" href="{{ post.url | relative_url }}">
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %-d" }}</time>
        <span>{{ post.title }}</span>
        <span aria-hidden="true">↗</span>
      </a>
  {% assign previous_year = current_year %}
  {% if forloop.last %}</div>{% endif %}
  {% endfor %}
</div>
