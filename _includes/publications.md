## Publications

{% for item in site.data.publications.main %}
  1. {% if item.image %} ![]({{ item.image }}) {% endif %}

     **{{ item.title }}**

     {{ item.authors }}

     {{ item.conference }}

     {% if item.pdf %} [[Paper]({{ item.pdf }})] {% endif %}
     {% if item.code %} [[Code]({{ item.code }})] {% endif %}
     {% if item.page %} [[Project Page]({{ item.page }})] {% endif %}
{% endfor %}
