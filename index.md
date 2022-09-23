---
title: My presentations
layout: base
---

 <!-- Tab links -->
<div class="tab">
  <button class="tablinks active" onclick="openCity(event, 'work')">work</button>
  <button class="tablinks" onclick="openCity(event, 'examples')">examples</button>
</div>

{% assign workprojects = "polifonia-facets-2022-09" | split: ','%}
{% assign examplesprojects = "adirondack-default,adirondack-xaprb,default,mutt,remarkwiki" | split: ','%}

<div id="work" class="tabcontent tabactive">
<ul>
{% for p in workprojects %}
<li><a href="/slides/work/{{ p }}/index.html#1">{{ p }}</a></li>
{% endfor %}
</ul>
</div>

<div id="examples" class="tabcontent">
<ul>
{% for e in examplesprojects %}
<li><a href="/slides/examples/{{ e }}/index.html#1">{{ e }}</a></li>
{% endfor %}
</ul>
</div>


