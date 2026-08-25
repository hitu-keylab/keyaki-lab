---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Keyaki Lab's Web Site
subtitle: 一橋大学 ソーシャル・データサイエンス学部/研究科 欅研究室
#permalink: /event/
#show_sidebar: true
---
## イベント一覧
<ul>
	{% for post in site.posts %}
		<li>
			<a href="{{ post.url | relative_url }}">{{ post.posttitle }}</a>
				: {{ post.author }}
				{{ post.date | date: "%Y-%m-%d" }}
		</li>
	{% endfor %}
</ul>
