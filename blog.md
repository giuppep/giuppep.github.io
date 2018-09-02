---
layout: default
title: blog
---
## latest posts
{% for post in site.posts %}

<div class="card clickable" markdown="1">
*{{ post.date | date_to_string }}*
{: .post_date}
### {{post.title}}
{: .post_title}
{% if post.description %}
{{post.description}}
{% else %}
{{post.excerpt}}
{% endif %}
<a href="{{post.url}}">read more...</a>
</div>

{% endfor %}
