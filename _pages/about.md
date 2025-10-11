---
permalink: /
title: "Yu Zhao's HomePage"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

-----------------------------------------------------------------------------
这是页面的“前言”部分，用于配置页面属性
-----------------------------------------------------------------------------
layout: about
title: About
permalink: / # 将此页面设置为主页 (homepage)

个人资料卡配置
profile:

你的头像照片路径。请将你的照片上传到 /assets/img/ 文件夹下
image: /assets/img/profile.jpg

图片在页面右侧或左侧显示
align: right

地址信息（可选）
address: > <p>123 University Avenue</p> <p>Your City, State 12345</p> <p>Your Institution</p>
About Me
Hello! I'm [Your Name], a [Your Position, e.g., Ph.D. candidate, Postdoctoral Researcher] in the [Your Department] at the [Your University].

My research focuses on the intersection of [Your Main Field 1] and [Your Main Field 2], with a special interest in [Your Specific Research Topic]. I am passionate about developing [e.g., novel algorithms, theoretical frameworks] to solve challenging real-world problems. I am fortunate to be advised by [Professor's Name(s)] and am a member of the [Your Lab or Research Group Name].

Before joining [Your University], I received my [Your Degree, e.g., M.S. in Computer Science] from [Previous University]. Feel free to explore my publications page for more details on my work.

Research Interests
[Research Interest 1: e.g., Machine Learning]

[Research Interest 2: e.g., Natural Language Processing]

[Research Interest 3: e.g., Generative AI]

[Research Interest 4: e.g., Computational Social Science]

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