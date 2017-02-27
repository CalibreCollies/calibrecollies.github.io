---
layout: collection
<!-- title: Over the rainbow bridge -->
permalink: /memory/
---

<h2 class="rainbow">Over the rainbow bridge</h2>

{% for item in site.memories %}
  {% if item.image %}
  <div class="row">
    <div class="small-8 columns">
      <h4>{{ item.title }}</h4>
      {{ item.content }}
    </div>
    <div class="small-4 columns">
      <img src="/assets/memories/{{ item.image }}" />
    </div>
  </div>
  {% else %}
  <div class="row item">
    <div class="small-12 columns">
      <h4>{{ item.title }}</h4>
      {{ item.content }}
    </div>
  </div>
  {% endif %}
  <hr />
{% endfor %}
