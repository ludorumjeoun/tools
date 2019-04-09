---
layout: page
title: Donors
permalink: /donors/
---

## 후원하기

{% include donation.html %}

## 후원자

{% for i in site.data.donor_scale %}
{% assign donors = site.data.donor | where_exp: "item", "item.scale == i" %}
{% if donors.size > 0 %}
### ${{ i }}
{% include donor_list.html donors=donors %}
{% endif %}
<br/>
{% endfor %}