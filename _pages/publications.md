---
layout: page
permalink: /publications/
title: Publications
description: "†: equally contributing authors"
nav: true
nav_order: 3
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}
{% include smcc_style.liquid %}

<style>
  /* Title + subtitle on the left, the filter box on the right, level with the title */
  .post-header {
    display: grid;
    grid-template-columns: 1fr auto;
    align-items: center;
    column-gap: 1.5rem;
  }
  .post-header .post-title,
  .post-header .post-description {
    grid-column: 1;
  }
  .post-header #bibsearch {
    grid-column: 2;
    grid-row: 1;
    align-self: center;
    width: 16rem;
    max-width: 40vw;
    margin: 0;
  }
  /* Gap between the submitted / to-be-submitted entries and the accepted / published ones */
  .publications .bibliography > li:has(.smcc-unpublished) + li:not(:has(.smcc-unpublished)) {
    margin-top: 3.5rem;
  }
  @media (max-width: 576px) {
    .post-header {
      display: block;
    }
    .post-header #bibsearch {
      width: 100%;
      max-width: none;
      margin-top: 0.75rem;
    }
  }
</style>

<script>
  // Move the filter box from the page body into the header row
  (function () {
    var input = document.getElementById("bibsearch");
    var header = document.querySelector(".post-header");
    if (!input || !header) return;
    var wrapper = input.parentElement;
    header.appendChild(input);
    if (wrapper && wrapper.tagName === "P" && !wrapper.textContent.trim()) wrapper.remove();
  })();
</script>

<div class="publications">

{% bibliography %}

</div>
