---
layout: default
title: About
permalink: /about/
---

<!-- {% include header2.html %}
<strong>Truncate words with 'truncatewords': </strong>

{{ "I enjoy Jekyll" | truncatewords: 2}}

<strong>Logic to detect current page ('if, elseif, else')</strong>
{% if page.title == 'About' %}
About page
{% elsif page.title == 'Home' %}
{% else %}
Other page
{% endif %}

<strong>Using 'unless' to detect page</strong>
{% unless page.title == "Contact" %}
It's not the contact page
{% endunless %}

{% include cta.html %} -->

<h1>About</h1>

Lorem ipsum dolor sit amet consectetur, adipisicing elit. Id repellendus nulla dolor recusandae cum officia molestiae? Dicta natus, dolorum quidem id unde labore voluptatem molestiae possimus saepe quis ipsum rerum!

<h3>More posts from this category:</h3>

<ul>
    {% for post in site.posts %}
        {% if post.categories contains "about" %}
        <li>
            <a href="{{ post.url }}">
                {{ post.title }}
            </a>
        </li>
        {% endif %}
    {% endfor %}
</ul>

<h3>More products from this category:</h3>

<ul>
    {% for product in site.data.products %}
        {% if product.category contains "about" %}
        <li>
            <a href="{{ product.url }}">
                {{ product.name }}
            </a>
        </li>
        {% endif %}
    {% endfor %}
</ul>