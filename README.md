# leaflet-freeze
>


## Description
Plugin for leaflet that freeze and thaw the leaflet map and all layers/objects on it

## Installation
### bower
`bower install https://github.com/FCOO/leaflet-freeze.git --save`

## Demo
http://FCOO.github.io/leaflet-freeze/demo/ 

## Usage

	map.freeze( [options] )
will prevent popup, contextmenu, click (optional), pan and zoom (optional) on the map and prevent popup, contextmenu, mouseover, mouseout, and dragging on the layers/objects on the map


	map.thaw();
will reset the map and the layers/objects

### New method

    L.Class.getHtmlElements: function() Return associated html-elements or array of Leaflet-elements



### options
| Id | Type | Default | Description |
| :--: | :--: | :-----: | --- |
| `allowZoomAndPan` | boolean | false | Allows zooming and panning on the map. If false the zoom-control is hidden
| `disableMapEvents` | string | "" | Names of events on the map to be disabled |
| `hideControls` | boolean | false | Hide all controls incl. zoom-control even if `options.allowZoomAndPan == true`|
| `hidePopups` | boolean | true | Close all open popups |
| `beforeFreeze` | function| null | Called before the map is 'freezed' |
| `afterThaw` | function| null | Called after the map is 'thawed' |
| `dontFreeze` |  object or []object | null | leaflet-object, html-element or array of ditto with element or "leaflet-owner" no to be frozen |

## Copyright and License
This plugin is licensed under the [MIT license](https://github.com/FCOO/leaflet-freeze/LICENSE).

Copyright (c) 2015 [FCOO](https://github.com/FCOO)

## Contact information

[Niels Holt](http://github.com/NielsHolt)

