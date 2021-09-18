---
layout: defaults/page
permalink: index.html
narrow: true
title: Welcome to my blog
---

## What is it?
- Đây sẽ là nơi lưu trữ những kiến thức mà tôi quan tâm trong những khoảng thời gian nhất định.
- Tôi lưu trữ nó nhằm mục đích xem lại khi cần.

## Recent Posts

{% for post in site.posts limit:3 %}
{% include components/post-card.html %}
{% endfor %}


