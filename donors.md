---
layout: page
title: Donors
permalink: donors
---

## 후원하기

{% include donation.html %}  
후원하신 분께서는 누락되거나, 잘못된 정보가 있을 경우 반드시 연락주세요.

## 후원자

{% for i in site.data.donor_scale %}
{% assign donors = site.data.donor | where_exp: "item", "item.scale == i" %}
{% if donors.size > 0 %}
### ${{ i }}
{% include donor_list.html donors=donors %}
{% endif %}
<br/>
{% endfor %}
