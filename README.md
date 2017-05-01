<section>
<ul>
{% for post in site.posts %}
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p><small><strong>{{ post.date | date: "%B %e, %Y" }}</strong><br>
        {{ post.excerpt | markdownify | strip_html | truncatewords:50 }}</small></p>
{% endfor %}
</ul>
</section>