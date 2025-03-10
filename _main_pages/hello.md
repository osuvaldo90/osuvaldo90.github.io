---
layout: default
emoji: 👋🏼
title: Hello
description: TODO
permalink: /
nav_order: 0
---

My name is Osuvaldo Ramos. Call me Osvi. I am a software engineer based in Philadelphia, PA.

What excites me most about software engineering is tackling complex problems and designing practical, elegant solutions to meet specific business needs. I have helped businesses automate processes, expand market reach, and build mission-critical systems that drive real results.

{% include variables.html %}

{% assign main_pages = main_pages | where_exp: "p", "p.url != page.url" %}
{% for p in main_pages %}
### {{ p.title }}
{{ p.excerpt }}
[Read more]({{ p.url }})
{% endfor %}

{%- comment -%} Take a look at my work or reach out to talk about interesting opportunities. {%- endcomment -%}
