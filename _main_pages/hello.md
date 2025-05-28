---
layout: default
emoji: 👋🏼
title: Hello
description: Senior Software Engineer in Philadelphia. Expert in TypeScript, domain-driven design, and scalable back-end systems. 10+ years of experience.
permalink: /
nav_order: 0
---

My name is Osuvaldo Ramos. Call me Osvi. I am a software engineer based in Philadelphia, PA. I enjoy tackling complex problems and designing practical, elegant solutions to meet specific business needs. Since 2013 I have helped businesses automate processes, expand market reach, and build mission-critical systems that drive real results.

{% include variables.html %}

{% assign sections = main_pages | where_exp: "p", "p.url != page.url" %}
{% for section in sections %}

### {{ section.title }}

{{ section.excerpt }}
[{{ section.read_more | default: "Read more" }}]({{ section.url }})
{% endfor %}

{%- comment -%} Take a look at my work or reach out to talk about interesting opportunities. {%- endcomment -%}
