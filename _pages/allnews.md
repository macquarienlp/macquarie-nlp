---
title: "News"
layout: textlay
excerpt: "Macquarie NLP group at Macquarie University."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<div style="margin-bottom: 15px;">
  <strong>{{ article.date }}</strong><br>
  <span style="font-size: 1.5em; font-weight: bold;">{{ article.headline | markdownify | strip_html }}</span>
  <div>{{ article.content | markdownify | strip_html }}</div>
</div>
{% endfor %}