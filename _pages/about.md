---
permalink: /
title: "Yu Zhao's HomePage"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

### About Me

My research focuses on the intersection of Generative AI and AI security. I am fortunate to be advised by Prof. [Ran He](https://rhe-web.github.io/) and Prof. [Jie Gui](https://guijiejie.github.io).


### Research Interests

[Research Interest 1: Generative AI]

[Research Interest 2: AI Security]

[Research Interest 3: Multi-modal Learning]

### Latest News & Posts
<!--
下面这段代码使用了 Jekyll Liquid 语法。
它会自动抓取并显示你在 _posts 文件夹中最新发布的 3 篇文章。
你不需要手动更新这里的内容。
-->

<div class="news">
{% for post in site.posts limit:3 %}
<div class="news-item">
<div class="news-date">
{{ post.date | date: "%b %d, %Y" }}
</div>
<div class="news-title">
<a href="{{ post.url | relative_url }}">{{ post.title }}</a>
</div>
</div>
{% endfor %}
</div>