---
layout: default
---
<h2>Writing</h2>
I write about culture, politics and technology. I'm always looking for new freelance opportunities, so <a href="mailto:dansinker@gmail.com">get in touch</a>. Here's what I've written in the last few years.
<ul>
{% for recent in site.data.recents %}
<li>{% if recent.writing == 'y' %}<a href="{{ recent.link }}">{{ recent.title }}</a> | {{ recent.publication }},  {{ recent.date | date: "%b %-d, %Y" }}{% endif %}
{% endfor %}