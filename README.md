# primitive-sphere

[![stable](http://badges.github.io/stability-badges/dist/stable.svg)](http://github.com/badges/stability-badges)

![screen](http://i.imgur.com/AJt2r8l.png)

A minimal UV sphere geometry for 3D rendering, including normals, UVs and cell indices. The algorithm has been adapted from [BabylonJS](https://github.com/BabylonJS/Babylon.js).

## Example

```js
var radius = 1
var mesh = require('primitive-sphere')(radius)

// the simplicial complex
console.log(mesh.positions, mesh.cells)

// rendering attributes
console.log(mesh.uvs)
console.log(mesh.normals)
```

## Usage

[![NPM](https://nodei.co/npm/primitive-sphere.png)](https://www.npmjs.com/package/primitive-sphere)

#### `mesh = sphere(radius, opt)`

Creates a new UV sphere mesh with the given `radius` (default 1) and options:

- `segments` number of segments to use, defaults to 32

## See Also

- [sphere-mesh](https://www.npmjs.com/package/sphere-mesh) - numerically robust
- [icosphere](https://www.npmjs.com/package/icosphere) - a simple icosphere simplicial complex

## License

MIT, see [LICENSE.md](http://github.com/glo-js/primitive-sphere/blob/master/LICENSE.md) for details.