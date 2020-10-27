---
layout: page
title: Lectures
permalink: /lectures/
---

Start: {{ site.course-start}}

End: {{ site.course-end}}

Week|Måndag|Tisdag |Onsdag |Torsdag|Fredag
-----|-------|-------|------|------|------
xx|01: 2020-08-31<br />[Lecture 1](lecture_01)<br />8:30 - 16:30|        |02: 2020-09-02<br />[Lecture 2](lecture_02)<br />8:30 - 16:30||


This page contains link to the lectures I give throughout the semester.


<ul id="archive">
{% for lecture in site.data.lectures %}
      <li class="archiveposturl">
        <span><a href="{{ lecture.slug }}">{{ lecture.title }}</a></span><br>
<span class = "postlower">
<strong>tl;dr:</strong> {{ lecture.tldr }}</span>
<strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:right; padding-right: .5em">
	<a href="https://github.com/{{ site.githubdir}}/tree/master/{{ lecture.dirname }}"><i class="fab fa-github"></i></a>&nbsp;&nbsp;
<a href="https://github.com/{{ site.githubdir}}/blob/master/{{ lecture.dirname }}/{{ lecture.filename}}.pdf"><i class="fas fa-file-pdf"></i></a>
</strong> 
      </li>
{% endfor %}
</ul>
