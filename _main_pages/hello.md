---
layout: default
emoji: 👋🏼
title: Hello
description: Senior Software Engineer in Philadelphia. Expert in TypeScript, domain-driven design, and scalable back-end systems. 10+ years of experience.
permalink: /
nav_order: 0
---

My name is Osvi and I'm a software engineer based in Philadelphia, PA.

I take a methodical and collaborative approach to problem solving that involves working with the team to truly understand what we're trying to solve and why before jumping into solutions. I believe this brings clarity and conviction during implementation.

Since 2013, I have worked in various industries including healthcare, real estate, and early childhood education and across many technologies from embedded systems to web applications.

{% include variables.html %}

{% assign sections = main_pages | where_exp: "p", "p.url != page.url" %}
{% for section in sections %}

## {{ section.title }}

{{ section.excerpt }}
[{{ section.read_more | default: "Read more" }}]({{ section.url }})
{% endfor %}

{%- comment -%} Take a look at my work or reach out to talk about interesting opportunities. {%- endcomment -%}
