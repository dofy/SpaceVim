---
title: "Blog"
description: "A list of latest blog about the feature of SpaceVim and tutorials of using vim."
---

# Blog

Here you can learn more about SpaceVim with our tutorials and find out what's
going on. Feel free to [feed this blog via RSS](../../feed.xml)：

<ul>
    {% for post in site.categories.blog %}
            <li>
               <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
               <span class="post-date">{{ post.date | date_to_string }}</span>
               <p>{{ post.excerpt | truncatewords: 100 }}</p>
            </li>
    {% endfor %}
</ul>
