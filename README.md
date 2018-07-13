# ol-hash

- This is modification [ol-hash](https://github.com/frogcat/ol-hash)([by frogcat](https://github.com/frogcat))

- OpenLayers v5 &amp; es6 support

# Usage

1.  `import { addHash } from './ol-hash'`
2.  call `addHash(map)`

# Example

## Code

```javascript
import { Map, View } from 'ol'
import { fromLonLat } from 'ol/proj'
import { Tile as TileLayer } from 'ol/layer/'
import { OSM } from 'ol/source/'

import { addHash } from './ol-hash'

const map = new Map({
  target: 'map',
  layers: [
    new TileLayer({
      source: new OSM()
    })
  ],
  view: new View({
    center: fromLonLat([132.601271, 34.232102], 'EPSG:3857'),
    zoom: 17.5
  })
})

addHash(map)
```
