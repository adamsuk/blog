---
title: Blog
content:
    items: '@self.children'
    limit: '10'
    order:
        by: date
        dir: desc
    pagination: '1'
    filter:
        type: item
---

Bloggy McBlogFace
<ul>
{% for p in page.parent.children if p != page %}
<li><a href="{{p.url}}">{{ p.title }}</a></li>
{% endfor %}
</ul>