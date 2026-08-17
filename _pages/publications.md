---
layout: archive
title: "Research"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% assign job_market_papers = site.publications | where: "category", "jmp" %}
<section class="research-section">
<h2 class="research-section__title">Job Market Paper</h2>
{% for post in job_market_papers reversed %}
{% include archive-single.html %}
{% endfor %}
</section>

{% assign published_papers = site.publications | where: "category", "publications" %}
<section class="research-section">
<h2 class="research-section__title">Publications</h2>
{% for post in published_papers reversed %}
{% include archive-single.html %}
{% endfor %}
</section>

{% assign working_papers = site.publications | where: "category", "working" %}
<section class="research-section">
<h2 class="research-section__title">Working Papers</h2>
{% for post in working_papers reversed %}
{% include archive-single.html %}
{% endfor %}
</section>

{% assign works_in_progress = site.publications | where: "category", "wip" %}
<section class="research-section">
<h2 class="research-section__title">Work in Progress</h2>
{% for post in works_in_progress reversed %}
{% include archive-single.html %}
{% endfor %}
</section>
