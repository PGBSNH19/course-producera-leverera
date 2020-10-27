---
layout: page
title: Lektioner
permalink: /lectures/
---

Start: {{ site.course-start}}, slut: {{ site.course-end}}

Vecka|Måndag|Tisdag|Onsdag|Torsdag|Fredag
-----|-------|-------|------{% for week in site.data.lectures %}
{{week.week}}{%- for day in week.days -%}|{% if day.lecture %}{{day.number}}: {{day.day}}<br />[{{day.lecture}}]({{day.slug}})<br />{{day.start-time}} - {{day.end-time}}{% endif %}{%- endfor -%}
{% endfor %}



## Alla lektioner
<ul id="archive">
{% for week in site.data.lectures %}
      <b>Vecka</b>: {{week.week}}<br/>
      
      {% for day in week.days %}
            {% if day.lecture %}

<li class="archiveposturl">
        <span><a href="{{ day.slug }}">{{ day.lecture }}</a></span><br>
<span class = "postlower">
{{ day.description }}</span>
<strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:right; padding-right: .5em">
	<a href="https://github.com/{{ site.githubdir}}/tree/master/{{ day.dirname }}"><i class="fab fa-github"></i></a>&nbsp;&nbsp;
<a href="https://github.com/{{ site.githubdir}}/blob/master/{{ day.dirname }}/{{ day.filename}}.pdf"><i class="fas fa-file-pdf"></i></a>
</strong> 
      </li>
            {% endif %}
      {% endfor %}
      
{% endfor %}
</ul>
