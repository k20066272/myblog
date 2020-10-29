---
layout: post
title:  "Archive of Chinese Artists"
date:   2020-10-29 18:05:00 +0800
categories: jekyll update
---

# Chinese Artists

{% for artist in site.data.artists %}
{{ artist.EnglishName  }}{{  artist.ChineseName  }} {{  artist.Nationality  }} ({{  artist.BirthYear  }}-{{  artist.DeathYear  }})

{% for i in (1..3) %}
 ![Artworks](/media/china-artworks/{{ artist.EnglishName | replace: " ", "_"}}_{{ artist.ChineseName }}/{{ artist.EnglishName | replace: " ", "_"}}_0{{ i }}.jpg)
{% endfor %}

{% endfor %}

