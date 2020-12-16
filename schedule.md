---
layout: page
title: Schema
permalink: /schedule/
---

Start: {{ site.course-start}}, slut: {{ site.course-end}}

Se även kalender på Confluence, dom borde vara i Sync, men är dom inte, då är det Confluence som gäller: [Dev kalender](https://plushogskolan.atlassian.net/wiki/display/TO/calendar/578442b2-ec9a-42c8-92c4-4ad20a003e69?calendarName=Dev)

Alla dagar i sprinterna har även [daily standup]({{ "/lectures/standup" | prepend: site.baseurl }}) även om dom inte syns här

Vecka|Måndag|Tisdag|Onsdag|Torsdag|Fredag
-----|-------|-------|------{% for week in site.data.schedule.weeks %}
{{week.week}}{%- for day in week.days -%}|{% if day.lectures %}**{{ day.lectures[0].start-full | date: "%F"}}**{%- for lecture in day.lectures -%}<br /><br />{{ lecture.start-full | date: "%R"}} - {{ lecture.end-full | date: "%R"}}<br />{{lecture.number}}: [{{lecture.lecture}}]({{lecture.slug}}){%- endfor -%}{% endif %}{%- endfor -%}
{% endfor %}



## Alla lektioner
<ul id="archive">
{% for week in site.data.schedule.weeks %}
      <b>Vecka</b>: {{week.week}}<br/>
      
      {% for day in week.days %}
            {% if day.lectures %}
{% for lecture in day.lectures %}
<li class="archiveposturl">
        <span class="postlower">{{ lecture.start-full | date: "%F"}} - {{day.weekday}}</span><br>
        <span><a href="{{ lecture.slug }}">{{ lecture.lecture }}</a></span><br>
<span class = "postlower">
{{ lecture.description }}</span>
<strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:right; padding-right: .5em">
	<a href="https://github.com/{{ site.githubdir}}/tree/master/{{ lecture.dirname }}"><i class="fab fa-github"></i></a>&nbsp;&nbsp;
<a href="https://github.com/{{ site.githubdir}}/blob/master/{{ lecture.dirname }}/{{ lecture.filename}}.pdf"><i class="fas fa-file-pdf"></i></a>
</strong> 
      </li>
      {% endfor %}
            {% endif %}
      {% endfor %}
      
{% endfor %}
</ul>
