---
layout: page
title: Home
id: home
permalink: /
---

# 저의 디지털 아카이브에 오신 것을 환영합니다.

###  [[about|About me / 소개]]

이 블로그를 Steph Ango 의 ['file-over-app'](https://stephango.com/file-over-app)에 영향을 받아 만들게 되었다.
Maxime Vaillancourt의 [github와 netlify를 이용한 블로그 만들기](https://maximevaillancourt.com/blog/setting-up-your-own-digital-garden-with-jekyll) 를 참고했다.

<strong> 최근에 발행된 노트 / Recently updated notes </strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 10 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>


<strong> you can find me elsewhere </strong>
- Twitter: [@laikainsputnik](https://x.com/LaikaInSputnik)
- bsky: [@laikainsputnik](https://bsky.app/profile/laikainsputnik.bsky.social)
- Instagram: [@skhim](https://www.instagram.com/skhim/)

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
