<div class="publications">
<ol class="bibliography">
{% for pub in site.data.publications.main %}
<li>
<div class="pub-row">
  <div class="col-sm-3 abbr">
    {% if pub.image %}<a href="{{ pub.image }}" target="_blank" rel="noopener"><img src="{{ pub.image }}" class="teaser" alt="{{ pub.image_alt | default: pub.title }}" loading="lazy"></a>{% endif %}
  </div>
  <div class="col-sm-9">
    <div class="title"><a href="{{ pub.url }}" target="_blank" rel="noopener">{{ pub.title }}</a></div>
    <div class="author">{{ pub.authors }}</div>
    <div class="periodical">{% if pub.workshop %}{{ pub.workshop }} @ <em>{{ pub.conference }}</em>{% else %}<em>{{ pub.venue }}</em>{% endif %}{% if pub.note %} · <em>{{ pub.note }}</em>{% endif %}</div>
    {% if pub.links %}<div class="links">{% for l in pub.links %}<a href="{{ l.url }}" class="btn" role="button" target="_blank" rel="noopener">{{ l.label }}</a>{% endfor %}</div>{% endif %}
    {% if pub.awards %}<div class="awards">{% for a in pub.awards %}<span class="award"><span class="award-kind">{{ a.kind }}</span>{% if a.venue %}<span class="award-venue">{{ a.venue }}</span>{% endif %}</span>{% endfor %}</div>{% endif %}
  </div>
</div>
</li>
{% endfor %}
</ol>
</div>
