---
layout: post
title: 'Extras'
comments: "These are just some extra things, not entirely needed, but as we keep going along certain topics have more explanations and new work. Read at your leisure..."
published: true
---

{{ page.comments }}

<div>
{% for thing in site.Theranos-markdown_notes %}
  {% if thing.type == 'Theranos-extra' %}
    <h3><a href="{{ thing.url | relative_url }}">{{ thing.title }}</a></h3><hr/>
  {% endif %}
{% endfor %}
{% assign uploads = site.static_files | where: 'Theranos-extra', true %}
{% for myuploads in uploads %}
  <h3><a href= "{{ site.baseurl }}/{{ myuploads.path }}">{{ myuploads.basename }}</a></h3><hr/>
{% endfor %}
</div>
