---
layout: default
title: 首页
---

# 我的个人日记

欢迎来到我的个人日记网站！这里记录了我的生活点滴、学习心得和感悟。

## 最近的日记

<div class="post-list">
{% for post in site.posts limit:5 %}
  <article class="post-item">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h2>
    <div class="post-meta">
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y年%m月%d日" }}</time>
      {% if post.mood %}<span class="post-mood">心情：{{ post.mood }}</span>{% endif %}
      {% if post.weather %}<span class="post-weather">天气：{{ post.weather }}</span>{% endif %}
    </div>
    <div class="post-excerpt">
      {{ post.excerpt | strip_html | truncatewords: 50 }}
    </div>
    {% if post.tags.size > 0 %}
      <div class="post-tags">
        {% for tag in post.tags %}
          <span class="tag">{{ tag }}</span>
        {% endfor %}
      </div>
    {% endif %}
  </article>
{% endfor %}
</div>

{% if site.posts.size > 5 %}
  <div style="text-align: center; margin-top: 2rem;">
    <a href="{{ '/archive/' | relative_url }}" class="more-posts">查看更多日记 →</a>
  </div>
{% endif %}

## 关于我

我是 MingXuan，一个热爱记录生活的人。通过写日记，我希望能够：

- 📝 记录生活中的美好瞬间
- 🎯 总结学习过程中的心得体会
- 💭 分享对生活的思考和感悟
- 🌱 追踪个人成长的轨迹

## 联系方式

- GitHub: [@rover-rock](https://github.com/rover-rock)
- Email: 362463215@qq.com
