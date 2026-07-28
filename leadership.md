---
layout: default
title: Leadership & Convening
---

# Leadership & Convening

Lynne organizes and directs recurring workshops and research convenings that connect academic research on electricity regulation and market design to practitioners and policymakers, and she serves in ongoing leadership and editorial roles across the field.

## Workshops & Events Directed

<ul class="entry-list">
{% for w in site.data.workshops.workshops %}
  <li>
    <strong>{{ w.title }}</strong>{% if w.org %}, {{ w.org }}{% endif %}
    {% if w.note %}<br><span class="entry-meta">{{ w.note }}</span>{% endif %}
    <br><span class="entry-meta">{{ w.years }}</span>
  </li>
{% endfor %}
</ul>

## Professional Leadership (Current)

<ul class="entry-list">
{% for l in site.data.leadership.current %}
  <li><strong>{{ l.role }}</strong>, {{ l.org }} <span class="entry-meta">({{ l.years }})</span></li>
{% endfor %}
</ul>

## Past Roles (Selected)

<ul class="entry-list">
{% for l in site.data.leadership.past %}
  <li>
    <strong>{{ l.role }}</strong>, {{ l.org }}{% if l.years != "" %} <span class="entry-meta">({{ l.years }})</span>{% endif %}
    {% if l.note %}<br><span class="entry-meta">{{ l.note }}</span>{% endif %}
  </li>
{% endfor %}
</ul>

## Hear & Read More

The video archive of past talks and presentations lives on the [YouTube channel]({{ site.youtube }}). For ongoing commentary and analysis, see [Knowledge Problem]({{ site.substack }}).
