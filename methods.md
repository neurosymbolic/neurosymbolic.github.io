---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

# layout: home
layout: page
title: Categorization of NS methods?
permalink: /methods/
---

# Categories:

5 categories from Pavans year start slides


Methods in each category etc. ..



Comparison of various methods etc ...





Neuro-symbolic is arguably the future of AI. It resolves many issues faced by deep learning and symbolic AI when used independently. Some of the benefits include: interpretability, learning from less resources, human-in-the-loop learning, and the ability to incorporate domain knowledge. Here we share the comments/reasons in support of neuro-symbolic AI from the leading experts and media.

<div class="container">
  <div class="row">
    <table class="table">
      {% for c in site.data.whyns %}
      <tr>
      <td><b>{{ c[1].summary }}</b> <br> <i> {{ c[1].author }}</i></td>
      <td><a href= "{{ c[1].url }}" > {{ c[1].publishedat }} </a></td>
      </tr>
      {% endfor %}
    </table>
  </div>
</div>
