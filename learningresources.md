---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

# layout: home
layout: page
title: Learning Resources
permalink: /learningresources/
---

<ul>
{% for l in site.data.learningresources %}
  <li>
    <a href="{{ l[1].url }}">{{ l[1].title }}</a>
    {% if l[1].details != "" %}
      {% if l[1].details contains "<ul>" %}
        {{ l[1].details }}
      {% else %}
        <ul><li>{{ l[1].details }}</li></ul>
      {% endif %}
    {% endif %}  
  </li>
{% endfor %}
</ul>
