---
layout: page
title: Posts
permalink: /posts/
---

# Blog Posts

Welcome to my blog! Here I share insights about software engineering, distributed systems, and technology trends.

## Recent Posts

{% for post in site.posts %}
  <article class="post">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}

{% if site.posts.size == 0 %}
## Coming Soon!

I'm currently working on some exciting blog posts about:

- **Distributed Systems Design Patterns**: Best practices for building scalable systems
- **Transaction Processing in Microservices**: Handling consistency in distributed environments
- **Message-Driven Architecture**: Building reactive systems with event sourcing
- **Performance Optimization**: Techniques for high-throughput applications

Stay tuned for updates! You can also follow my writing on:
- [Medium](https://medium.com/@ymanshur)
- [Substack](https://substack.com/@yusufmanshur869537)
{% endif %}