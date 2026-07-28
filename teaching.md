---
layout: default
title: Teaching, Advisory & Public Policy
---

# Teaching, Advisory & Public Policy

## Teaching

<h3>Graduate</h3>
<ul class="entry-list">
{% for c in site.data.teaching.graduate %}
  <li><strong>{{ c.course }}</strong> — {{ c.org }}</li>
{% endfor %}
</ul>

<h3>Undergraduate</h3>
<ul class="entry-list">
{% for c in site.data.teaching.undergraduate %}
  <li><strong>{{ c.course }}</strong> — {{ c.org }}</li>
{% endfor %}
</ul>

<h3>Freshman Seminars</h3>
<ul class="entry-list">
{% for s in site.data.teaching.freshman_seminars %}
  <li>{{ s }}</li>
{% endfor %}
</ul>

<p class="callout">The History of Economic Thought video channel (currently hosted on Vimeo) will be migrated here in a follow-on project — not part of this initial build.</p>

## Policy Research & Reports

<ul class="entry-list">
{% for r in site.data.policy_reports.reports %}
  <li>{{ r.year }}{% if r.month %} ({{ r.month }}){% endif %}. "{{ r.title }}." {{ r.publisher }}.</li>
{% endfor %}
</ul>

<p class="callout">Additional policy reports (2005–2025, per CV) to be added here.</p>

## Op-Eds & Media (Selected)

<p>Commentary published in outlets including:</p>
<ul class="entry-list">
{% for o in site.data.op_eds.outlets %}
  <li>{{ o }}</li>
{% endfor %}
</ul>

<p class="callout">Individual op-ed titles and dates (per CV) to be added here. Also see <a href="{{ site.substack }}">Knowledge Problem</a>, Lynne's newsletter since 2002.</p>

## Past Advisory Roles

<ul class="entry-list">
  <li><strong>Member</strong>, U.S. Department of Energy Electricity Advisory Committee <span class="entry-meta">(2021–2025)</span></li>
  <li><strong>Member</strong>, NIST Smart Grid Advisory Committee</li>
  <li><strong>Emerita</strong>, GridWise Architecture Council</li>
</ul>
