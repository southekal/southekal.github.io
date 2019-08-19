- <i class="fa fa-github" aria-hidden="true"></i> [github](https://github.com/southekal)
- <i class="fa fa-linkedin" aria-hidden="true"></i> [linkedin](https://linkedin.com/in/southe)
<ul>
  talks:
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
