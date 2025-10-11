---
permalink: /
title: "Yu Zhao's HomePage"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

My research focuses on the intersection of Generative AI and AI security. I am fortunate to be advised by Jie Gui and am a member of the Jie Group.


Research Interests
[Research Interest 1: Machine Learning]

[Research Interest 2: Natural Language Processing]

[Research Interest 3: Generative AI]

Latest News & Posts
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