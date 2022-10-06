---
layout: post
title: "TheranoXii | Materials"
permalink: /TheranoXii/
---

<span style="color:orange">Here are all the Theranos materials, files, links, etc...</span>

---

<!-- for the materials just put in headers for the topic: handouts, notes, and so on, the first example link is given, and the rest are just illustrations, feel free to edit as you may, the materials go in the 'course files' folder and you can add subfolders too! just be sure to reference the link correctly. you can also link to a post you made...-->

{% for item in site.data.materials.structure %}
  {% if item.show == true %}
  <h2><a href="{{ item.url }}">{{ item.title }}</a></h2>
  <hr/>
  {% endif %}
{% endfor %}
