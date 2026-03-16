---
title: Organizers
nav: true
---

# Organizers

<div class="people-grid-container">
  {% for person in site.data.organizers %}
    <div class="person">
      <div class="circle-crop-wrapper">
        <img src="{{ person.image | relative_url }}" alt="{{ person.name }}"
          {% if person.position %}
            style="object-position: {{ person.position }};"
          {% endif %}>
      </div>
      <h3>{{ person.name }}</h3>
      <p>{{ person.role }}</p>
      <p>{{ person.affiliation }}</p>
    </div>
  {% endfor %}
</div>

Hosted by [University of Idaho Library](http://www.lib.uidaho.edu/), {{ site.pub_year }}.
 
> built using [Jekyll](https://jekyllrb.com/) and [GitHub Pages](https://pages.github.com/)
>
> images and content: cc-by-sa <a href="https://github.com/{{ site.github_username }}">{{ site.author }}</a> {{ site.pub_year}} (get [source code]({{ site.repo }})).
> Last build date: {{ site.time | date: "%Y-%m-%d" }}.
>
> <a href="http://creativecommons.org/licenses/by-sa/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" alt="Creative Commons License" /></a>
