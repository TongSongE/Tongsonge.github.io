---
layout: default
work: true
main: true
title: Book
description: 좋았던 책을 리뷰합니다.
project-header: true
header-img: "img/project_bg.jpg"
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.book == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}
</div>
