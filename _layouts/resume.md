{% for js in page.customjs %}
<script async type="text/javascript" src="{{ js }}"></script>
{% endfor %}

{% include head.html %}
{{ content }}
