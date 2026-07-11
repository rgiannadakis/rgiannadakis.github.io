---
layout: page
title: Full CV
permalink: /full-cv/
---

{% assign about_page = site.pages | where: "url", "/" | first %}
{% assign cv_page = site.pages | where: "url", "/cv/" | first %}
{% assign pubs_page = site.pages | where: "url", "/publications/" | first %}
{% assign pres_page = site.pages | where: "url", "/presentations/" | first %}
{% assign teach_page = site.pages | where: "url", "/teaching/" | first %}

<div class="hero-grid full-cv-about">
  <div class="hero-left">
    <div class="hero-photo">
      <img class="avatar" src="/images/profile.png" alt="Rafail Giannadakis" onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';">
      <div class="avatar" style="display:none; align-items:center; justify-content:center; font-size:52px; color:var(--accent);">RG</div>
    </div>
  </div>
  <div class="hero-right">
    <h1 class="page-title full-cv-title">About</h1>
    <div class="prose prose--narrow">
      {{ about_page.content }}
    </div>
  </div>
</div>

<h1 class="page-title">{{ cv_page.title }}</h1>
{{ cv_page.content }}

<h1 class="page-title">{{ pubs_page.title }}</h1>
{{ pubs_page.content }}

<h1 class="page-title">{{ pres_page.title }}</h1>
{{ pres_page.content }}

<h1 class="page-title">{{ teach_page.title }}</h1>
{{ teach_page.content }}

<div class="btn-row no-print">
  <a class="btn btn-lg" href="javascript:window.print()">Save as PDF (Print)</a>
</div>