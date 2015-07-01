FusionTable-Map-custom-legend
=============================

Template to display Google Fusion Table Map with custom legend for non-numerical bucket categories. Consider this option if you need to create a map with textual legend labels (A, B, C) rather than numerical (0-50, 50-100). The instructions below explain how to simultaneously display map points/polygons using numerical data, and a custom legend using a matching column of textual data. 

This solution is necessary because Google Fusion Tables currently supports automatic legends ONLY for numerical data, in these cases:
- Point marker styles using buckets (numerical data only)
- Polygon fill color styles using buckets or gradients (numerical data only)

Learn more at https://support.google.com/fusiontables/answer/185991

Based on code from Google https://developers.google.com/fusiontables/docs/samples/legend

##Demos:
1) Point map with Google's sample fusion table (butterflies) http://jackdougherty.github.io/FusionTable-Map-custom-legend/butterflies.html

2) *NOT working* Point map with user uploaded fusion table (markets) http://jackdougherty.github.io/FusionTable-Map-custom-legend/markets.html 

to come** polygon version, dynamic version

##Instructions for point maps 

1) Design your Google Fusion Table with two parallel data columns, such as TypeText (such as A, B, C) and TypeNumber (1, 2, 3), and also a Location column (such as addresses, or two columns of latitude & longitude coordinates). In each row, the TypeText must match your TypeNumber (e.g. A = 1, B = 2, etc.), and if you change one value, you must change the other. For basics on designing Google Fusion Table maps, see my Data Visualization book at http://epress.trincoll.edu/dataviz

2) Create your Google Fusion Table, create the Map, change feature styles, select points > marker icon > buckets, and choose your numerical data column (such as TypeNumber). Change settings to display your colored points on the map. Do NOT create an automatic legend here.

3) Change sharing settings to make your Google Fusion Table Map public, or visible to those who receive a link.

4) Obtain a copy of the template file (such as points.html) from this GitHub repository. Either fork it to your own free GitHub account, or clone it to your desktop with GitHub for Mac/Windows, or download the zip file. One advantage to creating your own free GitHub account is that you will need to edit and host your own version on the public web, which is convenient to do with the GitHub Pages feature, but requires learning some additional steps. See details at http://epress.trincoll.edu/dataviz

4) Modify the template HTML file. Look for lines commented with "MODIFY" to insert your preferred title, map center and zoom level, Google Fusion Table ID number and Location column, and the content and colors for your legend. For your legend, display your non-numerical data column (such as TypeText). One advantage to doing all of this in GitHub is the built-in code editor. Or you can use any text editing tool on your desktop.

5) Host your new template file on a web server. One advantage to using GitHub is its Pages features, which is how I display the Demo sites above.

##Polygon maps are similar in design: see
- http://www.mulinblog.com/tutorial-embed-a-google-fusion-tables-map-with-a-legend-to-a-wordpress-post
- http://gmaps-samples.googlecode.com/svn/trunk/fusiontables/legend_template.html

##See also
- Searchable Map Template by @DerekEder at http://derekeder.com/searchable_map_template/, which is a more sophisticated solution to the non-numerical legend category problem
