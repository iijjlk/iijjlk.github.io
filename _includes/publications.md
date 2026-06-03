## Publications

{% for item in site.data.publications.main %}
<div class="publication">
  {% if item.image %}
  <img src="{{ item.image }}" class="pub-img">
  {% endif %}
  <div class="pub-text">
    <strong>{{ item.title }}</strong><br>
    {{ item.authors }}<br>
    <em>{{ item.conference }}</em><br>
    {% if item.pdf %}<a href="{{ item.pdf }}">[Paper]</a>{% endif %}
    {% if item.code %}<a href="{{ item.code }}">[Code]</a>{% endif %}
    {% if item.page %}<a href="{{ item.page }}">[Project Page]</a>{% endif %}
  </div>
</div>
{% endfor %}
