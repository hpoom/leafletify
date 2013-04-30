Leafletify
==========

A simple jQuery plugin to plot map points using schema.org markup for points (http://schema.org/Place).

You can have multiple points on a map & multiple maps with multiple points all from one call to leafletify();

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
	<h1>Holiday Extras building (the 'wave')</h1>
	<p>The company I work for.</p>
	<div itemprop="geo" itemscope itemtype="http://schema.org/GeoCoordinates">
		<meta itemprop="latitude" content="51.086535" />
		<meta itemprop="longitude" content="1.034732" />
	</div>
</div>

<div itemscope itemtype="http://schema.org/Place" class="mapItem" data-mapid="myMap" data-popover="true">
	<h1>Royal Oak</h1>
	<p>The building I work in.</p>
	<div itemprop="geo" itemscope itemtype="http://schema.org/GeoCoordinates">
		<meta itemprop="latitude" content="51.08571" />
		<meta itemprop="longitude" content="1.035612" />
	</div>
</div>
```

HTML (map container)
--------------------
```html
<div id="myMap"></div>
```