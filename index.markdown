---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<div id="blog-posts">

{% for post in site.posts %}
	<article class="post">
		{% if post.external-url %}
	    	<h1>
				<a href="{{ post.external-url }}">{{ post.title }}</a> 
				<a class="anchor" href="{{ post.url }}"><i class="icon-anchor"></i></a>
			</h1>
		{% else %}
        		<h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
		{% endif %}
	</article>
{% endfor %}
</div>