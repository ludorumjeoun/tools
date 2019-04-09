---
layout: page
title: About
permalink: /about/
---

Ludorum의 블로그 겸, 유틸리티 프로그램을 모아둔 사이트입니다.  
주로 기술적인 내용과 함께 최근 관심있게 보는 블록체인과 관련된 내용들을 다루고 있습니다.

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