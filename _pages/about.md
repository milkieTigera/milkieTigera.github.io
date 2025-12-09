---
permalink: /
title: "Yu Zhao's HomePage"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

### About Me

My research focuses on the intersection of Generative AI and AI security. I am fortunate to be advised by Prof. [Ran He](https://rhe-web.github.io/), Prof. [Keke Gai](https://cst.bit.edu.cn/szdw/jsml/bssds/3600ddc31a2e4daa99c3a3c3be802f1b.htm) and Prof. [Jie Gui](https://guijiejie.github.io).


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