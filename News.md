---
title: News Archive
permalink: /News/
---

# News Archive

<div class="news">
  <ul class="news-timeline">
    {% assign sorted_news = site.data.news | sort: 'date' | reverse %}
    {% for new in sorted_news %}
      <li class="timeline-item">
        <span class="timeline-date">{{ new.date | date: "%b %d, %Y" }}</span>
        <span class="timeline-dot"></span>
        <span class="timeline-content">{{ new.details }}</span>
      </li>
    {% endfor %}
  </ul>
</div>
