---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

# layout: home
layout: page
title: Publication Venues
permalink: /venues/
---

<h1 id="ConfWkshop"> Conferences and Workshops </h1>

<div class="container">
  <div class="row">
    <table class="table">
      <tr>
      <th>Name (URL)</th>
      <th>Sumbission Date</th>
      <th>Conference Date/Venue</th>
      <th>Comments</th>
      </tr>
      {% for c in site.data.conferences %}
      <tr>
      <td><a href= "{{ c[1].url }}" > {{ c[1].abbr }} </a> <br> {{c[1].title}} </td>
      <td>{{ c[1].subdate }}</td>
      <td>{{ c[1].confdate }} <br> {{ c[1].venue }}</td>
      <td>{{ c[1].comment }}</td>
      </tr>
      {% endfor %}
    </table>
  </div>
</div>

# Journals


<div class="container">
  <div class="row">
    <table class="table">
      <tr>
      <th>Name (URL)</th>
      <th>Comments</th>
      </tr>

      {% for j in site.data.journals %}
      <tr>
      <td><a href= "{{ j[1].url }}" > {{ j[1].abbr }} </a> <br> {{j[1].title}} </td>
      <td>{{ j[1].comment }}</td>
      </tr>
      {% endfor %}
    </table>
  </div>
</div>


<!--- <ul>
{% for c in site.data.conf %}
  <li>
  {{c[1].abbr}}
  {{c[1].title}}
  </li>
{% endfor %}
</ul>
-->
