---
layout: page
---

## Software Projects 

<div class="posts" id="Blog">
    <ul style="padding-left: 0em">
        {% assign software-projects = site.software-projects | sort | reverse %}
        {% for software-project in software-projects %}
        <li>
            <div style="font-weight: normal"><a href="{{ site.baseurl }}{{ software-project.url }}">{{ software-project.title | downcase }}</a>: {{ software-project.description | downcase }}</div>
        </li>
        {% endfor %}
    </ul>
</div>
