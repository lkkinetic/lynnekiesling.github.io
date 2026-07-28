---
layout: default
title: Home
---

# Lynne Kiesling

<p class="tagline-lede">{{ site.tagline }}</p>

Lynne Kiesling is an economist specializing in electricity market design, regulatory institutions, and the economics of technological change in network industries. Drawing on the economics of knowledge and information, institutional and transaction cost analysis, mechanism design, and complexity theory, she analyzes how regulatory frameworks adapt—or fail to adapt—when technology changes faster than the institutions governing it. Her empirical and theoretical work spans wholesale power market design and performance, resource adequacy, transactive energy systems, distributed energy resources, and price-based automation at varying scales in power systems.

As Director of Northwestern's Institute for Regulatory Law and Economics, she leads a translational research program connecting academic scholarship to the practice of state utility regulation. As External Faculty at the Santa Fe Institute, she applies complexity economics to the co-evolution of energy technology and regulatory institutions. Her policy work—including analysis for the American Enterprise Institute and (past) the U.S. Department of Energy's Electricity Advisory Committee—bridges academic rigor and regulatory practice, engaging audiences from state commissions to FERC. She publishes regularly at [Knowledge Problem]({{ site.substack }}).

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

## Contact & Links

<ul class="entry-list">
  <li><a href="mailto:{{ site.email }}">{{ site.email }}</a></li>
  <li><a href="mailto:{{ site.email_northwestern }}">{{ site.email_northwestern }}</a></li>
  <li><a href="{{ site.scholar }}">Google Scholar</a></li>
  <li><a href="{{ site.ssrn }}">SSRN Author Page</a></li>
  <li><a href="{{ site.orcid }}">ORCID: 0000-0002-6854-2653</a></li>
  <li><a href="{{ '/cv.html' | relative_url }}">Curriculum Vitae</a></li>
</ul>
