---
layouts: pages
---

# Discountry & IFE

This is my baidu IFE task notes & codes site.

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
