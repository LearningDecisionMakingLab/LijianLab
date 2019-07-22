---
title: Publications
layout: page
group: publications
---


<div class="container-fluid">

<div class="row" style="padding-top: 60px; margin-top: -60px;">

<br>

{% assign sorted = site.data.publications | sort: 'published_at' |reverse %}

{% for publication in sorted %}

{{ publication.title | markdownify }}

{% if publication.pdf %}

 <a href = "{{publication.pdf}}" alt = "PDF"> <b>PDF</b></a>

{% endif %}

<br>
<br>

{% endfor %}

</div>
</div>
