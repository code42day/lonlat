[![NPM version][npm-image]][npm-url]
[![Build Status][travis-image]][travis-url]
[![Dependency Status][gemnasium-image]][gemnasium-url]

# lonlat

Converters for various coordinate representations.

## Install

```sh
$ npm install --save lonlat
```

## Usage

```js
var lonlat = require('lonlat');

lonlat.geojson.centerSphere();
lonlat.mongo.toPoly();
```

### `geojson` methods always return geojson shape or collection of shapes

- `centerSphere`- create a Sphere corresponding to inscribed circle
- `multiPolygon` - create a Polygon from the string of coordinates
- `polygon` - create a Polygon from the string of coordinates
- `shapesArray` - split boxes into Polygons and Multipolygons
- `splitBox` - split box into grid of Polygons


### `mongo` methods return coordinates pairs [lon,lat] that can be indexed by mongo

- `toLonLat`
- `toPoly`
- `toBox`
- `toBoxes`

## License

MIT © [Damian Krzeminski](https://pirxpilot.me)

[npm-image]: https://img.shields.io/npm/v/lonlat.svg
[npm-url]: https://npmjs.org/package/lonlat

[travis-url]: https://travis-ci.org/pirxpilot/lonlat
[travis-image]: https://img.shields.io/travis/pirxpilot/lonlat.svg

[gemnasium-image]: https://img.shields.io/gemnasium/pirxpilot/lonlat.svg
[gemnasium-url]: https://gemnasium.com/pirxpilot/lonlat
