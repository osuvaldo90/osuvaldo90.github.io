---
layout: default
emoji: 👋🏼
title: Hello
description: Senior Software Engineer | TypeScript, Node.js, PostgreSQL | REST APIs & Backend Systems | 10+ Years
permalink: /
nav_order: 0
---

I'm a Senior Software Engineer with over 10 years of experience building production backend systems using TypeScript, Node.js, and PostgreSQL. I specialize in designing RESTful APIs, GraphQL schemas, and scalable cloud-native architectures that solve complex business problems.

I'm a Senior Software Engineer with over 10 years of experience building production backend systems using TypeScript, Node.js, and PostgreSQL. I specialize in designing RESTful APIs, GraphQL schemas, and scalable cloud-native architectures that solve complex business problems.

I started programming at age 12 and never stopped. What drives me is the satisfaction of building software that makes a real difference. Whether that's enabling home ownership for thousands of families, helping educators run childcare programs, or supporting patients with medication adherence.

{% include variables.html %}

{% assign sections = main_pages | where_exp: "p", "p.url != page.url" %}
{% for section in sections %}

## {{ section.title }}

{{ section.excerpt }}
[{{ section.read_more | default: "Read more" }}]({{ section.url }})
{% endfor %}

{%- comment -%} Take a look at my work or reach out to talk about interesting opportunities. {%- endcomment -%}
