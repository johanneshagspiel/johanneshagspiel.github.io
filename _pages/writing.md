---
layout: page
---

## Writing 

<div class="posts" id="Blog">
    <ul style="padding-left: 0em">
        {% assign writings = site.writing | sort | reverse %}
        {% for writing in writings %}
        <li>
            <div style="font-weight: normal"><a href="{{ site.baseurl }}{{ writing.url }}">{{ writing.title | downcase }}</a>: {{ writing.description | downcase }}</div>
        </li>
        {% endfor %}
    </ul>
</div>
