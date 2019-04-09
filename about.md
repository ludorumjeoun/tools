---
layout: page
title: About
permalink: /about/
---

Ludorum의 블로그 겸, 유틸리티 프로그램을 모아둔 사이트입니다.  
주로 기술적인 내용과 함께 최근 관심있게 보는 블록체인과 관련된 내용들을 다루고 있습니다.

### 기술 문의
기술적인 문의는 최소 1,000원 후원과 함께 받고있습니다. **후원 후 문의주세요.**

{% for address in site.data.address %}
- <span class="sans"><b>{{ address.symbol }}</b> `{{ address.address }}`</span>
{% endfor %}
- <b class="sans">[카카오 페이](https://qr.kakaopay.com/2810060110000028190677901f408435)</b>

<script>
    function telegram() {
        // 스팸 방지
        window.open(atob("aHR0cHM6Ly90Lm1lL2x1ZG9ydW0="));
    }
</script>
<b><a href="javascript:telegram();">&gt; Telegram 문의하기</a></b>

### 문의 내역
<table>
{% for donor in site.data.donor reversed %}
    <tr><th colspan="2">{{ donor.date | replace: "-", "년 " }}월</th></tr>
{% for category in donor.category %}
    <tr><td>{{ category.name }} 문의</td><td>{{ category.count }}건</td></tr>
{% endfor %}
{% endfor %}
</table>