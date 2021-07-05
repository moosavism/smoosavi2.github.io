---
layout: page
permalink: /talks/
title: Talks
description: Most recent invited talks.
year: [2019]
nav: true
---

<div class="publications">

{% for y in page.year %}
  <!--h2 class="year">{{y}}</h2-->
  {% bibliography -f talks -T talk -q @*[year>={{y}}]* %}
{% endfor %}

</div>
