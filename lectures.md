---
layout: page
title: Lektioner
permalink: /lectures/
---

Start: {{ site.course-start}}, slut: {{ site.course-end}}

Vecka|Måndag|Tisdag |Onsdag |Torsdag|Fredag
-----|-------|-------|------|------|------
50|01: 2020-12-07<br />[Lecture 1](lecture_01)<br />8:30 - 16:30|02: 2020-12-08<br />[Workshop](workshop)<br />Team 1<br />8:30 - 16:30|03: 2020-12-09<br />[Workshop](workshop)<br />Team 2<br />8:30 - 16:30|04: 2020-12-10<br />[Workshop](workshop)<br />Team 3<br />8:30 - 16:30|05: 2020-12-11<br />[Workshop](workshop)<br />Team 4<br />8:30 - 16:30
51|06: 2020-12-14<br />[Lecture 2](lecture_02)<br />8:30 - 15:30|07: 2020-12-15<br />[Standup](standup)<br />8:30 - 11:00|08: 2020-12-16<br />[Standup](standup)<br />8:30 - 11:00|09: 2020-12-17<br />[Standup](standup)<br />8:30 - 11:00|10: 2020-12-18<br />[Standup](standup)<br />8:30 - 11:00
52|11: 2020-12-21<br />[Lecture 3](lecture_03)<br />8:30 - 15:30|12: 2020-12-22<br />[Standup](standup)<br />8:30 - 11:00|13: 2020-12-23<br />[Standup](standup)<br />8:30 - 11:00||
53|14: 2020-12-28<br />[Lecture 4](lecture_04)<br />8:30 - 15:30|15: 2020-12-29<br />[Standup](standup)<br />8:30 - 11:00|16: 2020-12-30<br />[Standup](standup)<br />8:30 - 11:00||
01|17: 2021-01-04<br />[Lecture 5](lecture_05)<br />8:30 - 15:30|18: 2021-01-04<br />[Standup](standup)<br />8:30 - 11:00||19: 2021-01-05<br />[Standup](standup)<br />8:30 - 11:00|20: 2021-01-08<br />[Standup](standup)<br />8:30 - 11:00
02|21: 2021-01-11<br />[Lecture 6](lecture_06)<br />8:30 - 15:30|22: 2021-01-12<br />[Standup](standup)<br />8:30 - 11:00|23: 2021-01-13<br />[Standup](standup)<br />8:30 - 11:00|24: 2021-01-14<br />[Standup](standup)<br />8:30 - 11:00|25: 2021-01-15<br />[Standup](standup)<br />8:30 - 11:00
03|26: 2021-01-18<br />[Lecture 7](lecture_07)<br />8:30 - 15:30|27: 2021-01-19<br />[Standup](standup)<br />8:30 - 11:00|28: 2021-01-20<br />[Standup](standup)<br />8:30 - 11:00|29: 2021-01-21<br />[Presentation](presentation)<br />8:30 - 11:00|30: 2021-01-22<br />[Tenta](tenta)<br />9:00 - 13:00



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
