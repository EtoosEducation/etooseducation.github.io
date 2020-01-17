---
layout: default
title: "Etoos Tech Blog"
main: true
subtitle: Etoos Tech Blog Main
post-header: true
---

<ul class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.blog == true %}
{% include post-list.html %}
{% endif %}
{% endfor %}
</ul>