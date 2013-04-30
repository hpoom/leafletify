Leafletify
==========

A simple jQuery plugin to plot map points using schema.org markup. Each 'place' (http://schema.org/Place)

# Usage #

Libraries for leaflet.js to work
--------------------------------
```html
<link rel="stylesheet" href="http://cdn.leafletjs.com/leaflet-0.5/leaflet.css" />
 <!--[if lte IE 8]>
     <link rel="stylesheet" href="http://cdn.leafletjs.com/leaflet-0.5/leaflet.ie.css" />
 <![endif]-->
<script src="http://cdn.leafletjs.com/leaflet-0.5/leaflet.js"></script>
<script type="text/javascript" src="/path/to/jQuery.leafletify.js"></script>
```

jQuery
--------
```javascript
$('.mapItem').leafletify();
```

Points (each item you want to appear on map)
------------------------------------------
```html
<div itemscope itemtype="http://schema.org/Place" class="mapItem" data-mapid="myMap" data-popover="true">
	<h1>TITLE</h1>

	<p>Some text etc etc</p>

	<div itemprop="geo" itemscope itemtype="http://schema.org/GeoCoordinates">
		<meta itemprop="latitude" content="51.086535" />
		<meta itemprop="longitude" content="1.034732" />
	</div>
</div>
```

HTML (map container)
--------------------
```html
<div id="myMap"></div>
```