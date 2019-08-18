# Sandip Southekal
- [github](https://github.com/southekal)
- [linkedin](https://linkedin.com/in/southe)
- talks

<ul>
  <b>{{ site.posts }}</b>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
