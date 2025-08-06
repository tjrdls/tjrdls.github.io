---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default     # 테마에 맞는 레이아웃 이름 넣기 (예: default, page 등)
title: 블로그 글 목록
---

# 블로그 글 목록

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      - {{ post.date | date: "%Y-%m-%d" }}
    </li>
  {% endfor %}
</ul>

[LinkedIn 프로필]({{ site.linkedin_url }})