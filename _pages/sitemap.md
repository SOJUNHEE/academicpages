---
layout: archive
title: "사이트맵"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

이 사이트의 모든 페이지입니다. 검색엔진용 [XML 사이트맵]({{ base_path }}/sitemap.xml)도 있습니다.

<h2>페이지</h2>
{% for post in site.pages %}{% if post.title and post.url != '/404.html' %}
  {% include archive-single.html %}
{% endif %}{% endfor %}

<h2>프로젝트</h2>
{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}
