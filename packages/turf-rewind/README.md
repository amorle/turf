# @turf/rewind

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## rewind

Rewind [(Multi)LineString][1] or [(Multi)Polygon][2] outer ring counterclockwise and inner rings clockwise (Uses [Shoelace Formula][3]).

### Parameters

*   `geojson` **[GeoJSON][4]** input GeoJSON Polygon
*   `options` **[Object][5]** Optional parameters (optional, default `{}`)

    *   `options.reverse` **[boolean][6]** enable reverse winding (optional, default `false`)
    *   `options.mutate` **[boolean][6]** allows GeoJSON input to be mutated (significant performance increase if true) (optional, default `false`)

### Examples

```javascript
var polygon = turf.polygon([[[121, -29], [138, -29], [138, -18], [121, -18], [121, -29]]]);

var rewind = turf.rewind(polygon);

//addToMap
var addToMap = [rewind];
```

Returns **[GeoJSON][4]** rewind Polygon

[1]: https://tools.ietf.org/html/rfc7946#section-3.1.4

[2]: https://tools.ietf.org/html/rfc7946#section-3.1.6

[3]: http://en.wikipedia.org/wiki/Shoelace_formula

[4]: https://tools.ietf.org/html/rfc7946#section-3

[5]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object

[6]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean

<!-- This file is automatically generated. Please don't edit it directly:
if you find an error, edit the source file (likely index.js), and re-run
./scripts/generate-readmes in the turf project. -->

---

This module is part of the [Turfjs project](http://turfjs.org/), an open source
module collection dedicated to geographic algorithms. It is maintained in the
[Turfjs/turf](https://github.com/Turfjs/turf) repository, where you can create
PRs and issues.

### Installation

Install this module individually:

```sh
$ npm install @turf/rewind
```

Or install the Turf module that includes it as a function:

```sh
$ npm install @turf/turf
```
