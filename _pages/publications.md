---
layout: page
permalink: /publications/
title: Publications
description: List of my published work.
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

<h1>Manuscript</h1>
{% bibliography --query @article %}

<h1>Thesis</h1>
{% bibliography --query @book %}

<h1>Conference Proceedings</h1>
{% bibliography --query @inproceedings %}


</div>
