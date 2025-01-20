---
title: test page
---
- only show the note with a category "자전거"
- You can find some grammers here
    https://shopify.github.io/liquid/

<ul>
  {% for note in site.notes %}
    {% if "자전거" == note.category %}
        <li>
       {{ note.last_modified_at | date: "%Y-%m-%d" }} - <a href="{{ note.url }}">{{ note.title }}</a>
        </li>
    {% endif %}
  {% endfor %}
</ul>

### 일기 모음
<ul>
  {% for note in site.notes %}
    {% if "journal" == note.category %}
        <li>
       {{ note.last_modified_at | date: "%Y-%m-%d" }} - <a href="{{ note.url }}">{{ note.title }}</a>
        </li>
    {% endif %}
  {% endfor %}
</ul>
