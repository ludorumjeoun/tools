---
layout: page
title: Contact
permalink: /contact
---

### 기술 문의
기술적인 문의는 최소 1,000원 후원과 함께 받고있습니다. **후원 후 문의주세요.**

{% include donation.html %}

### 문의 내역
<table>
{% for inquiry in site.data.inquiry reversed %}
    <tr><th colspan="2">{{ inquiry.date | replace: "-", "년 " }}월</th></tr>
{% for category in inquiry.category %}
    <tr><td>{{ category.name }} 문의</td><td>{{ category.count }}건</td></tr>
{% endfor %}
{% endfor %}
</table>
