---
layout: page
title: Lektioner
permalink: /lectures/
---

Start: {{ site.course-start}}, slut: {{ site.course-end}}

Vecka|Måndag|Tisdag |Onsdag |Torsdag|Fredag
-----|-------|-------|------|------|------
50|01: 2020-12-07<br />[Lecture 1](lecture_01)<br />8:30 - 15:30|02: [Workshop](workshop)<br />Team 1|03: [Workshop](workshop)<br />Team 2|04: Workshop<br />Team 3|05: [Workshop](workshop)<br />Team 4
51|06: 2020-12-14<br />[Lecture 2](lecture_02)<br />8:30 - 15:30|07: [Standup](standup)|08: [Standup](standup)|09: [Standup](standup)|10: [Standup](standup)
52|11: 2020-12-21<br />[Lecture 3](lecture_03)<br />8:30 - 15:30|12: [Standup](standup)|13: [Standup](standup)||
53|14: 2020-12-28<br />[Lecture 4](lecture_04)<br />8:30 - 15:30|15: [Standup](standup)|16: [Standup](standup)||
01|17: 2021-01-04<br />[Lecture 5](lecture_05)<br />8:30 - 15:30|18: [Standup](standup)||19: [Standup](standup)|20:[Standup](standup)
02|21: 2021-01-11<br />[Lecture 6](lecture_06)<br />8:30 - 15:30|22: [Standup](standup)|23: [Standup](standup)|24: [Standup](standup)|25: [Standup](standup)
03|26: 2021-01-18<br />[Lecture 7](lecture_07)<br />8:30 - 15:30|27: [Standup](standup)|28: [Standup](standup)|29: [Presentation](presentation)|30: [Tenta](tenta)



## Alla lektioner
<ul id="archive">
{% for lecture in site.data.lectures %}
      <li class="archiveposturl">
        <span>{{lecture.date}} <a href="{{ lecture.slug }}">{{ lecture.title }}</a></span><br>
<span class = "postlower">{{ lecture.description }}</span>
<strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:right; padding-right: .5em">
	<a href="https://github.com/{{ site.githubdir}}/tree/master/{{ lecture.dirname }}"><i class="fab fa-github"></i></a>&nbsp;&nbsp;
<a href="https://github.com/{{ site.githubdir}}/blob/master/{{ lecture.dirname }}/{{ lecture.filename}}.pdf"><i class="fas fa-file-pdf"></i></a>
</strong> 
      </li>
{% endfor %}
</ul>
