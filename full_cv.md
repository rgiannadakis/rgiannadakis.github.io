---
layout: page
title: Curriculum Vitae
permalink: /full-cv/
---

{% assign about_page = site.pages | where: "url", "/" | first %}
{% assign cv_page = site.pages | where: "url", "/cv/" | first %}
{% assign pubs_page = site.pages | where: "url", "/publications/" | first %}
{% assign pres_page = site.pages | where: "url", "/presentations/" | first %}
{% assign teach_page = site.pages | where: "url", "/teaching/" | first %}

<div class="plain-cv">

<div class="cv-header">
  <img class="avatar" src="/images/profile.png" alt="Rafail Giannadakis" onerror="this.style.display='none';">
  <h1>Rafail Giannadakis</h1>
  <p class="contact-line">
  giannadakis.uni@gmail.com &middot; rgiannadakis@ucsb.edu &middot;
  <a href="https://www.linkedin.com/in/rgiannadakis">LinkedIn</a> &middot;
  <a href="https://orcid.org/0009-0009-6708-4396">ORCID</a> &middot;
  <a href="https://crete.academia.edu/RafailGiannadakis">Academia.edu</a>
  </p>
</div>

<h2 class="cv-section">About</h2>
<div class="prose">
{{ about_page.content | markdownify }}
</div>

<hr class="cv-divider">
<h2 class="cv-section">{{ cv_page.title }}</h2>
<div class="prose">
{{ cv_page.content | markdownify }}
</div>

<hr class="cv-divider">
<h2 class="cv-section">{{ pubs_page.title }}</h2>
<div class="prose">
{{ pubs_page.content | markdownify }}
</div>

<hr class="cv-divider">
<h2 class="cv-section">{{ pres_page.title }}</h2>
<div class="prose">
{{ pres_page.content | markdownify }}
</div>

<hr class="cv-divider">
<h2 class="cv-section">{{ teach_page.title }}</h2>
<div class="prose">
{{ teach_page.content | markdownify }}
</div>

</div>

<div class="btn-row no-print">
  <a class="btn btn-lg" href="javascript:window.print()">Save as PDF (Print)</a>
</div>