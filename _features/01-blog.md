---
id: Blog
name: Blog
heading: Blog
image: "images/brain.jpg"
---

<div class="home">

  <ul class="post-list">
    {% for post in site.posts %}
        <h3>
          <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}:</span>
            <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h3>
    {% endfor %}
  </ul>

</div>
