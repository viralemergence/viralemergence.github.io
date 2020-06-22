---
layout: base
title: Home
---



<script>
$(document).ready(function() {
    $('#main').DataTable( {
        columnDefs: [ {
            targets: [ 0 ],
            orderData: [ 0, 1 ]
        }, {
            targets: [ 1 ],
            orderData: [ 1, 0 ]
        }, {
            targets: [ 4 ],
            orderData: [ 4, 0 ]
        } ]
    } );
} );
</script>




<body>

<table id="main" class="display" style="width:100%">
  <thead>
  <tr>
    <th> Species </th>
    <th> Betacov </th>
    <th> Trait1 </th>
    <th> Trait2 </th>
    <th> Trait3 </th>
    <th> Network1 </th>
    <th> Network2 </th>
    <th> Network3 </th>
    <th> Network4 </th>
    <th> Ensemble </th>
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






