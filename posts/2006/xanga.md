---
date: 2006-01-01
title: Xanga archives
layout: layouts/post.njk
templateEngineOverride: md,njk,html
---

This is an archive of Xanga posts from 2005-2006. I was only 15, so please bear with the grammar and content.

{% for post in xanga %}
<h2>{{ post.post_date | readableDataDateTime}}</h2>
{{ post.content | jsonToHtml }}
{% endfor %}