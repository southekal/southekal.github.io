- <i class="fa fa-github" aria-hidden="true"></i> [github](https://github.com/southekal)
- <i class="fa fa-linkedin" aria-hidden="true"></i> [linkedin](https://linkedin.com/in/southe)
- <i class="fas fa-book-open"></i> talks:
  - [cypress - end to end testing tool](https://southekal.com/talks/cypress-presentation.html)

<ul>
  {% if site.posts %}
  	posts: {{ site.posts }}
  {% endif %}
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
