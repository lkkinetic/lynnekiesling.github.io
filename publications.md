---
layout: default
title: Publications
---

# Publications

## Books

<ol class="entry-list">
{% for b in site.data.books.books %}
  <li>{{ b.authors }}. {{ b.year }}. <em>{{ b.title }}</em>. {{ b.publisher }}.</li>
{% endfor %}
</ol>

## Edited Volumes

<ol class="entry-list">
{% for b in site.data.books.edited_volumes %}
  <li>{{ b.authors }}. {{ b.year }}. <em>{{ b.title }}</em>. {{ b.publisher }}.</li>
{% endfor %}
</ol>

{% if site.data.books.chapters and site.data.books.chapters.size > 0 %}
## Book Chapters

<ol class="entry-list">
{% for c in site.data.books.chapters %}
  <li>{{ c.authors }}. {{ c.year }}. "{{ c.title }}." In <em>{{ c.in }}</em>.</li>
{% endfor %}
</ol>
{% else %}
## Book Chapters

<p class="callout">Selected book chapters (2014–2021, per CV) to be added here.</p>
{% endif %}

## Articles (Peer-Reviewed, Selected, 2007–2026)

<ol class="entry-list">
{% for a in site.data.publications.articles %}
  <li>
    {{ a.authors }}. {{ a.year }}. "{{ a.title }}."
    <em>{{ a.journal }}</em>{% if a.volume %} {{ a.volume }}{% endif %}{% if a.note %} ({{ a.note }}){% endif %}.
    {% if a.url %}<a href="{{ a.url }}">{{ a.url }}</a>{% endif %}
  </li>
{% endfor %}
</ol>

<p class="callout">Earlier publications and a complete list are available via <a href="{{ site.ssrn }}">SSRN</a> and <a href="{{ site.scholar }}">Google Scholar</a>.</p>

## Working Papers &amp; Current Projects

<h3>Working Papers</h3>
<ul class="entry-list">
{% for w in site.data.working_papers.working_papers %}
  <li>{{ w.title }} <span class="entry-meta">({{ w.note }})</span></li>
{% endfor %}
</ul>

<h3>Current Projects</h3>
<ul class="entry-list">
{% for p in site.data.working_papers.current_projects %}
  <li><strong>{{ p.name }}</strong> — {{ p.description }} <span class="entry-meta">({{ p.funder }})</span></li>
{% endfor %}
</ul>

<h3>Current Grants</h3>
<ul class="entry-list">
{% for g in site.data.grants.grants %}
  <li>{{ g.funder }}, "{{ g.title }}" — {{ g.role }} <span class="entry-meta">({{ g.years }}, {{ g.amount }})</span></li>
{% endfor %}
</ul>
