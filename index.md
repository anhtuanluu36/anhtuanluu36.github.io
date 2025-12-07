---
layout: default
---

<div class="home">
  <section class="hero">
    <h1 class="page-heading">{{ site.title }} - Blog</h1>
    <p class="hero-description">Updates on my projects, apps, and development journey</p>
  </section>

  {% if site.posts.size > 0 %}
  <section class="blog-posts">
    <h2>Latest Updates</h2>
    <div class="post-list">
      {% for post in site.posts %}
        <article class="post-preview">
          <header class="post-preview-header">
            <h3>
              <a class="post-link" href="{{ post.url | relative_url }}">
                {{ post.title | escape }}
              </a>
            </h3>
            <div class="post-meta">
              <time datetime="{{ post.date | date_to_xmlschema }}">
                {{ post.date | date: "%B %d, %Y" }}
              </time>
              {% if post.categories.size > 0 %}
                <span class="post-categories">
                  {% for category in post.categories %}
                    <span class="category">{{ category }}</span>
                  {% endfor %}
                </span>
              {% endif %}
              {% if post.tags.size > 0 %}
                <span class="post-tags">
                  {% for tag in post.tags limit:3 %}
                    <span class="tag">#{{ tag }}</span>
                  {% endfor %}
                </span>
              {% endif %}
            </div>
          </header>

          <div class="post-excerpt">
            {% if post.excerpt %}
              {{ post.excerpt | strip_html | truncate: 300 }}
            {% else %}
              {{ post.content | strip_html | truncate: 300 }}
            {% endif %}
          </div>

          <footer class="post-preview-footer">
            <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
          </footer>
        </article>
      {% endfor %}
    </div>
  </section>
  {% else %}
  <section class="no-posts">
    <h2>Coming Soon</h2>
    <p>I'll be sharing updates about my projects and development journey soon. Stay tuned!</p>

    <div class="quick-about">
      <h3>About Me</h3>
      <p>
        I'm Luu Anh Tuan, a software developer passionate about mobile applications,
        NFC technology, and creating tools that solve real-world problems.
        Follow this blog for updates on my NFC Tool app and other projects.
      </p>
      <a href="{{ '/about/' | relative_url }}" class="btn">Learn More About Me</a>
    </div>
  </section>
  {% endif %}

  <section class="blog-sidebar">
    <div class="widget">
      <h3>Categories</h3>
      <div class="categories">
        <span class="category-item">App Updates</span>
        <span class="category-item">Development</span>
        <span class="category-item">NFC Technology</span>
        <span class="category-item">Tutorials</span>
        <span class="category-item">Personal</span>
      </div>
    </div>

  </section>
</div>