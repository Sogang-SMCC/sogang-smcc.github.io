---
layout: about
title: Welcome
permalink: /

selected_papers: false
social: false

announcements:
  enabled: false

latest_posts:
  enabled: false
---

{% include smcc_style.liquid %}

<style>
  .home-intro figure {
    margin: 0 0 1.75rem;
  }
  .home-address {
    font-size: 15px;
    line-height: 1.45;
  }
  .home-address p {
    margin: 0;
  }
  @media (max-width: 767px) {
    .home-address .col-md-6 + .col-md-6 {
      margin-top: 1rem;
    }
  }
</style>

<div class="home-intro">
  {% include figure.liquid path="assets/img/smcc/campus.png" class="img-fluid rounded z-depth-1 w-100" alt="Sogang University" %}
</div>

<div class="row home-address">
  <div class="col-md-6">
    <p><strong>Soft Matter Computational Chemistry Lab</strong><br>
    Ricci Science Hall 1217, 1215<br>
    Department of Chemistry, Sogang University<br>
    Seoul 04107, Korea<br>
    TEL: 82-2-716-8889<br>
    e-mail: <a href="mailto:bjsung@sogang.ac.kr">bjsung@sogang.ac.kr</a></p>
  </div>
  <div class="col-md-6">
    <p>서강대학교 화학과 리치과학관 1217호, 1215호<br>
    서울특별시 마포구 백범로 35<br>
    전화: 02-716-8889<br>
    이메일: <a href="mailto:bjsung@sogang.ac.kr">bjsung@sogang.ac.kr</a></p>
  </div>
</div>
