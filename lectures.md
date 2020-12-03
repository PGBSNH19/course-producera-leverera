---
layout: page
title: Schema
permalink: /schedule/
---

Start: {{ site.course-start}}, slut: {{ site.course-end}}

Vecka|Måndag|Tisdag|Onsdag|Torsdag|Fredag
-----|-------|-------|------{% for week in site.data.lectures %}
{{week.week}}{%- for day in week.days -%}|{% if day.lectures %}**{{day.day}}**{%- for lecture in day.lectures -%}<br /><br />{{lecture.start-time}} - {{lecture.end-time}}<br />{{lecture.number}}: [{{lecture.lecture}}]({{lecture.slug}}){%- endfor -%}{% endif %}{%- endfor -%}
{% endfor %}



## Alla lektioner
<ul id="archive">
{% for week in site.data.lectures %}
      <b>Vecka</b>: {{week.week}}<br/>
      
      {% for day in week.days %}
            {% if day.lectures %}
{% for lecture in day.lectures %}
<li class="archiveposturl">
        <span class="postlower">{{day.day}} - {{day.weekday}}</span><br>
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
