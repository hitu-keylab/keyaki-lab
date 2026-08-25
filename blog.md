---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Keyaki Lab's Web Site
subtitle: 一橋大学 ソーシャル・データサイエンス学部/研究科 欅研究室
#permalink: /event/
#show_sidebar: true
---
<style>
.event-meta {
  font-size: 0.8em;
  color: #777;
  margin-left: 0.4em;
}
</style>

## イベント一覧
<ul>
	{% for post in site.posts %}
		<li>
			<a href="{{ post.url | relative_url }}">{{ post.posttitle }}</a>
			<span class="event-meta">
				{% if post.author %}
					: {{ post.author }}
				{% endif %}
				- <span>{{ post.date | date: "%Y-%m-%d" }}
			</span>
		</li>
	{% endfor %}
</ul>
