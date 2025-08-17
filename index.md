# Latest Posts

Welcome to the SkyNetHosting blog — practical, no‑fluff hosting guides to speed up your sites and grow your business.

{% assign posts_list = site.posts | sort: 'date' | reverse %}
<ul class="post-list">
  {% for post in posts_list %}
  <li>
    <a class="post-title" href="{{ post.url }}">{{ post.title }}</a>
    <span class="post-date">{{ post.date | date: "%b %d, %Y" }}</span>
    <p class="excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
  </li>
  {% endfor %}
</ul>

{% include cta.html text="Try our high‑performance hosting — 50% off for 3 months" link="https://skynethosting.net/signup?utm_source=github&utm_medium=blog&utm_campaign=home-cta" %}
