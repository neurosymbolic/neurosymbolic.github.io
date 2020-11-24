---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

# layout: home
layout: page
title: Publications
permalink: /publications/
---

# Survey papers

<ul>
{% for p in site.data.publications %}
  {% if p[1].type == "survey" %}
    <li>
    {{p[1].author}}.
    <b>{{p[1].title}}</b>,
    {{p[1].publishedat}},
    {{p[1].year}},
    <a href="{{ p[1].url }}">{{ p[1].url }}</a>
    {% if p[1].comment != "" %}
      ({{p[1].comment}})
    {% endif %}  
    </li>
   {% endif %}
{% endfor %}
</ul>
