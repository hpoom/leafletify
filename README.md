Leafletify
==========

A simple jQuery plugin to plot map points using schema.org markup

# Usage #


HTML
----

__Points__
<div itemscope itemtype="http://schema.org/Place" class="mapItem" data-mapid="map1" data-mapicondiv="icon1">
	<div itemprop="geo" itemscope itemtype="http://schema.org/GeoCoordinates">
		<meta itemprop="latitude" content="123456" />
		<meta itemprop="longitude" content="765432" />
	</div>
</div>

__Map__
<div class="map" id="map1" data-zoomlevel="12"></div>


Jquery
------
$( '.mapItem' ).leafletify()

