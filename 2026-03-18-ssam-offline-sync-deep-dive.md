
---
layout: default
---
<article class="post">
  <header class="post-header">
    <h1 class="post-title">{{ page.title }}</h1>
    <p class="post-meta">{{ page.date | date: "%b %-d, %Y" }} • Tags: {% for tag in page.tags %}<a href="/tags/#{{ tag | slugify }}">#{{ tag }}</a>{% if forloop.last == false %}, {% endif %}{% endfor %}</p>
  </header>
  <div class="post-content">{{ content }}</div>
</article>
