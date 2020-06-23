---
layout: base
title: Home
---




<body>


<table id="table" class="display"  style="width:100%">
  <thead>
  <tr>
    <th> Species </th>
    <th> Training data </th>
    <th> New data </th>
    <th> Ensemble </th>
    <th> Trait.1 </th>
    <th> Trait.2 </th>
    <th> Trait.3 </th>
    <th> Hybrid </th>
    <th> Network.1 </th>
    <th> Network.2 </th>
    <th> Network.3 </th>
    <th> Network.4 </th>
    <th> Source </th>
  </tr>
  </thead>

  <tbody>
  {% for row in site.data.predictions %}
	{% if forloop.first %}
  {% endif %}
  {% tablerow pair in row %}
    {{ pair[1] }}
  {% endtablerow %}
  {% endfor %}

  </tbody>
</table>

</body>






