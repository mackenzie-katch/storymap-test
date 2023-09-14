<div id="mapdiv" style="width: 100%; height: 600px;"></div>

<!-- Your script tags should be placed before the closing body tag. -->
<link rel="stylesheet" href="https://mackenzie-katch.github.io/storymap-test/i-41-stylesheet.css">
<script type="text/javascript" src="https://cdn.knightlab.com/libs/storymapjs/latest/js/storymap-min.js"></script>

<script>
// storymap_data can be an URL or a Javascript object
var storymap_data = 'https://mackenzie-katch.github.io/storymap-test/published.json';

// certain settings must be passed within a separate options object
var storymap_options = {};

var storymap = new KLStoryMap.StoryMap('mapdiv', storymap_data, storymap_options);
window.onresize = function(event) {
    storymap.updateDisplay(); // this isn't automatic
}
</script>

<!-- in page settings code -->
<!-- Mapbox with CMS markers -->
<script>
    // Replace with your own Mapbox access token
    mapboxgl.accessToken = 'pk.eyJ1IjoiZGV2b3JtYXBzIiwiYSI6ImNsN3FqMnowYTA1ZTUzbm12dXk3dWR0dGoifQ.mJBt7snqZSbKh3F0Jpcssg';


      const map = new mapboxgl.Map({
        container: 'map',
        // You can change the style url below with your own style from Mapbox
        style: 'mapbox://styles/devormaps/clesnxlxj000b01lpd9kfv7lf',
        center: [-88.46637725830078, 44.28699443765375],
        zoom: 10.85
      });


    // Call the function to initialize the map
    initializeMap();
  </script>
