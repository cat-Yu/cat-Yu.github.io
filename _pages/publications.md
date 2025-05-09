---
layout: page
permalink: /publications/
title: Publications
description: \* equal contribution
nav: true
nav_order: 1
---
### Peer-Reviewed Conference and Journal Papers
<!-- _pages/publications.md -->
<div class="publications">

{% bibliography -f {{ site.scholar.bibliography }} --query @*[paper=true]* %}
</div>

### LBWs, Workshops
<div class="publications">
{% bibliography -f {{ site.scholar.bibliography }} --group_by none --query @*[paper=false]* %}
</div>

