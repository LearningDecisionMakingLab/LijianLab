---
title: Collaborators
layout: page
group: links
---



<div class="container-fluid">

<div class="row" style="padding-top: 60px; margin-top: -60px;">

<br>

<!-- not sure how the sort function works here -->

{% assign sorted = site.data.collaborators | sort: 'abbreviation'%}


{% for collaborator in sorted %}

{{ collaborator.name}}, {{collaborator.education}}, <i>{{ collaborator.school}}</i>

{% if collaborator.website %}

 <a href = "{{collaborator.website}}" alt = "website"> [web]</a>

{% endif %}

<br>
<br>

{% endfor %}

</div>
</div>
