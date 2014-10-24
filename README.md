FusionTable-Map-custom-legend
=============================

Template to display Google Fusion Table Map with custom legend for non-numerical bucket categories. Consider this option if you need to create a map with textual legend labels (A, B, C) rather than numerical (0-50, 50-100).

Based on code from Google https://developers.google.com/fusiontables/docs/samples/legend

Demos:
Google sample point map (North America butterflies) http://jackdougherty.github.io/points.html

My Connecticut sample point map (ADD**) http://jackdougherty.github.io/points-ct.html

to come** polygon versions

Quick instructions:

1) Design your Google Fusion Table with two parallel data columns, such as TypeText (such as A, B, C) and TypeNumber (1, 2, 3), and also a Location column (such as addresses, or two columns of latitude & longitude coordinates). For basics on designing Google Fusion Table maps, see my Data Visualization book at http://epress.trincoll.edu/dataviz

2) Create your Google Fusion Table, create the Map, change the map style (*check wording), and use Buckets using TypeNumber

