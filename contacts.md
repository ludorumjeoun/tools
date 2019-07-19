---
layout: page
title: Contacts
permalink: contacts
---

### 기술 문의
기술적인 문의는 최소 1,000원 후원과 함께 받고있습니다. **후원 후 문의주세요.**

{% include donation.html %}

#### If you want share critical secrets with me, use PGP or [Keybase@ludorum](https://keybase.io/encrypt#ludorum)
```
-----BEGIN PGP PUBLIC KEY BLOCK-----
Comment: https://keybase.io/ludorum
Version: Keybase Go 3.1.2 (darwin)

xjMEXK2DghYJKwYBBAHaRw8BAQdAPrWqulzWHfqm57MAZox7YGMEYucZ1dBOa57Z
X+sX+FrNIkx1ZG9ydW0gSmVvdW4gKElEKSA8bHVkb3J1bUBwbS5tZT7CcwQTFggA
JQUCXK2DggkQdOyoNqlUOPoCGwMFCwkIBwIGFQoJCAsCBBYCAwEAAHl0AQA76+uN
gIRy7vqWaoeZO+xo9xq8rEHUdB2XYvTr1tu4AwEAezo3hkkKbKBaugA150FfVgC1
dzwK1ylHADl2cow1CQbOOARcrYOCEgorBgEEAZdVAQUBAQdAc6oHTnfxXT/TwIQp
qP/V/D8XVc9G+e6I0/ROmunUTwUDAQgHwngEGBYIACAWIQSngdc8jGgrc/GnMNp0
7Kg2qVQ4+gUCXK2DggIbDAAKCRB07Kg2qVQ4+kbcAQDdFlBHxVMk2AyEOqJby1sC
31QDm1V9lRCo6Hnv3Xi5JwD/TNgyWiyjNKaHpgoZirRYEUKsOTenOMRsfH+liXua
nAI=
=XyUm
-----END PGP PUBLIC KEY BLOCK-----
```

### 문의 내역
<table>
{% for inquiry in site.data.inquiry reversed %}
    <tr><th colspan="2">{{ inquiry.date | replace: "-", "년 " }}월</th></tr>
{% for category in inquiry.category %}
    <tr><td>{{ category.name }} 문의</td><td>{{ category.count }}건</td></tr>
{% endfor %}
{% endfor %}
</table>
