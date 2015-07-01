FusionTable-Map-custom-legend
=============================

This HTML template displays Google Fusion Table maps with custom text legend for non-numerical bucket categories. Consider this option if you need to create a map with textual legend labels (A, B, C) rather than numerical (0-50, 50-100). Currently, Google Fusion Tables supports automatic legends ONLY for numerical data, such as point map marker icons using buckets, and polygon map fill color styles using buckets or gradients. This template allows you to display text labels in your map legend, by pairing this text column with a numerical column in your Google Fusion Table. 

##Demo:
Point map of US market locations at http://jackdougherty.github.io/FusionTable-Map-custom-legend/

See also the underlying Google Fusion Table at  https://www.google.com/fusiontables/DataSource?docid=1RXgs33--EUO1ARJsNr0VQwju9TyebQpkuBlbxmlF

##To Do:
- polygon version: for now, see samples at http://gmaps-samples.googlecode.com/svn/trunk/fusiontables/legend_template.html and http://www.mulinblog.com/tutorial-embed-a-google-fusion-tables-map-with-a-legend-to-a-wordpress-post
- dynamic version

##Credits:
- Point map based on code from Google https://developers.google.com/fusiontables/docs/samples/legend
- With coding help from Karen_J in the GFT Google Products Forum
- Thanks to Bryant Dowd for the market location data

##Point map instructions

1) Design your Google Fusion Table with two parallel data columns, such as TypeText (such as A, B, C) and TypeNumber (1, 2, 3), and also a Location column (such as a geocoded addresses, or two columns of latitude & longitude coordinates). In each row, the TypeText must match your TypeNumber (e.g. A = 1, B = 2, etc.), and if you change one value, you must change the other. For basics on designing Google Fusion Table maps, see my Data Visualization book at http://epress.trincoll.edu/dataviz

2) Create your Google Fusion Table, create the Map, change feature styles, select points > marker icon > buckets, and choose your numerical data column (such as TypeNumber). Change settings to display your colored points on the map. Do NOT create an automatic legend here.

3) Change sharing settings to make your Google Fusion Table Map public, or visible to those who receive a link.

4) Obtain a copy of the template file (such as points.html) from this GitHub repository. Either fork it to your own free GitHub account, or clone it to your desktop with GitHub for Mac/Windows, or download the zip file. One advantage to creating your own free GitHub account is that you will need to edit and host your own version on the public web, which is convenient to do with the GitHub Pages feature, but requires learning some additional steps. See details at http://epress.trincoll.edu/dataviz

4) Modify the template HTML file. Look for lines commented with "MODIFY" to insert:
- your preferred title
- map center and zoom level
- header of your geocoded location data column
- Google Fusion Table ID number (see File > About this Table)
- styleId and templateId to match your colored markers and info window (see Map > Publish > Get JavaScript and HMTL)
- text labels and colors for your legend (to match those in your Table and your Map feature styles)
For your legend, display your non-numerical data column (such as TypeText). One advantage to doing all of this in GitHub is the built-in code editor. Or you can use any text editing tool on your desktop.

5) Host your new template file on a web server. One advantage to using GitHub is its Pages features, which is how I display the Demo sites above.

##See also
- Searchable Map Template by @DerekEder at http://derekeder.com/searchable_map_template/, which is a more sophisticated solution to the non-numerical legend category problem
