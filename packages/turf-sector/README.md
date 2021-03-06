# @turf/sector

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## sector

Creates a circular sector of a circle of given radius and center [Point](https://tools.ietf.org/html/rfc7946#section-3.1.2),
between (clockwise) bearing1 and bearing2; 0 bearing is North of center point, positive clockwise.

**Parameters**

-   `center` **[Coord](https://tools.ietf.org/html/rfc7946#section-3.1.1)** center point
-   `radius` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** radius of the circle
-   `bearing1` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** angle, in decimal degrees, of the first radius of the sector
-   `bearing2` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** angle, in decimal degrees, of the second radius of the sector
-   `options` **[Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)** Optional parameters (optional, default `{}`)
    -   `options.units` **[string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)** miles, kilometers, degrees, or radians (optional, default `'kilometers'`)
    -   `options.steps` **[number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number)** number of steps (optional, default `64`)
    -   `options.properties` **Properties** Translate properties to Feature Polygon (optional, default `{}`)

**Examples**

```javascript
var center = turf.point([-75, 40]);
var radius = 5;
var bearing1 = 25;
var bearing2 = 45;

var sector = turf.sector(center, radius, bearing1, bearing2);

//addToMap
var addToMap = [center, sector];
```

Returns **[Feature](https://tools.ietf.org/html/rfc7946#section-3.2)&lt;[Polygon](https://tools.ietf.org/html/rfc7946#section-3.1.6)>** sector polygon

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
$ npm install @turf/sector
```

Or install the Turf module that includes it as a function:

```sh
$ npm install @turf/turf
```
