---
layout: page
title: About
description: 学习使我快乐
keywords: 小张同学 Yuqi Zhang
comments: true
menu: 关于
permalink: /about/
---

Hi！I am a first-year master student in Statistics at University of Illinois

我爱学习，学习使我快乐。

和优秀的人在一起，你会变得更优秀。

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
