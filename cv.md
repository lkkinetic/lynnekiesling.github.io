---
layout: default
title: CV
---

# Curriculum Vitae

<p class="callout">
  Download: <a href="{{ '/assets/cv/Kiesling_CV.pdf' | relative_url }}">Kiesling_CV.pdf</a>
  &mdash; <strong>placeholder link.</strong> Drop your current CV PDF into
  <code>assets/cv/Kiesling_CV.pdf</code> in the repo to make this link live.
</p>

## Contact

- {{ site.email }}
- {{ site.email_northwestern }}
- [{{ site.url }}]({{ site.url }})
- ORCID: [0000-0002-6854-2653]({{ site.orcid }})
- [Knowledge Problem]({{ site.substack }})
- SSRN: [{{ site.ssrn }}]({{ site.ssrn }})
- Google Scholar: [{{ site.scholar }}]({{ site.scholar }})

## Current Appointments

<ul class="entry-list">
{% for a in site.data.appointments.current %}
  <li><strong>{{ a.role }}</strong>, {{ a.org }}{% if a.years != "" %} <span class="entry-meta">({{ a.years }})</span>{% endif %}</li>
{% endfor %}
</ul>

## Past Appointments

<ul class="entry-list">
{% for a in site.data.appointments.past %}
  <li><strong>{{ a.role }}</strong>, {{ a.org }} <span class="entry-meta">({{ a.years }})</span></li>
{% endfor %}
</ul>

## Education

<ul class="entry-list">
{% for e in site.data.appointments.education %}
  <li>{{ e.degree }}, {{ e.org }} <span class="entry-meta">({{ e.year }})</span></li>
{% endfor %}
</ul>

## Books & Edited Volumes

<ul class="entry-list">
{% for b in site.data.books.books %}
  <li>{{ b.authors }}. {{ b.year }}. <em>{{ b.title }}</em>. {{ b.publisher }}.</li>
{% endfor %}
{% for b in site.data.books.edited_volumes %}
  <li>{{ b.authors }}. {{ b.year }}. <em>{{ b.title }}</em>. {{ b.publisher }}.</li>
{% endfor %}
</ul>

## Peer-Reviewed Articles (Selected)

<p>See the full list on the <a href="{{ '/publications.html' | relative_url }}">Publications</a> page.</p>

## Working Papers, Current Projects & Grants

<p>See the <a href="{{ '/publications.html' | relative_url }}">Publications</a> page.</p>

## Teaching

<p>See the <a href="{{ '/teaching.html' | relative_url }}">Teaching, Advisory & Public Policy</a> page.</p>

## Workshops Directed & Professional Leadership

<p>See the <a href="{{ '/leadership.html' | relative_url }}">Leadership & Convening</a> page.</p>
