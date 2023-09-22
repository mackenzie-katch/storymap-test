<div id="mapdiv" style="width: 100%; height: 600px;"></div>

<!-- Your script tags should be placed before the closing body tag. -->
<link rel="stylesheet" href="https://mackenzie-katch.github.io/storymap-test/i-41-stylesheet.css">
<script type="text/javascript" src="https://cdn.knightlab.com/libs/storymapjs/latest/js/storymap-min.js"></script>
  <script src="http://unpkg.com/leaflet@latest/dist/leaflet.js"></script>
  <script src="js/leaflet-providers.js"></script>
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
