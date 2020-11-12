---
layout: post
title:  "Heavy Metal Bands"
date:   2020-11-12 18:05:00 +0800
categories: jekyll update
---

# All Bands

<h1>Decades</h1>
- [Bands formed 1960s](/bands/1960s.html)
- [Bands formed 1970s](bands/1970s.markdown)
- [Bands formed 1980s]
- [Bands formed 1990s]
- [Bands formed 2000s]

{% for band in site.data.metal_bands_2017 %}
<p><h1>{{ band.band_name  }}</h1>({{  band.formed  }}-{{  band.DeathYear  }})</p>
<p>Fans Number: {{  band.fans  }}</p>
<p>Origin: {{  band.origin  }}</p>
<p>Band Split: {{  band.split  }}</p>
<p>Band Style: {{  band.style  }}</p>


{% endfor %}

