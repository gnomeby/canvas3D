PLY 3D model viewer based on HTML5 canvas
=========================================

3D HTML5 canvas realization based on 2D and WebGL context.

Examples:
* 2D: [Cube](http://gnomeby.github.com/canvas3D/canvas-3d-cube.html) (see **Cube function** in source code)
* 2D: [Suzanne monkey](http://gnomeby.github.com/canvas3D/canvas-ply-reader.html?file=monkey.ply)
* 2D: [Utah teapot](http://gnomeby.github.com/canvas3D/canvas-ply-reader.html?file=teapot.ply)
* WebGL: [Suzanne monkey](http://gnomeby.github.com/canvas3D/webgl-ply-reader.html?file=monkey.ply)
* WebGL: [Utah teapot](http://gnomeby.github.com/canvas3D/webgl-ply-reader.html?file=teapot.ply)

Features:
* 3D operations: rotating, moving object center
* Ambient light (only WebGL)
* Directional light
* Perspetive camera (only WebGL)
* Highlighting edges (only 2D)
* Painter's algorithm for sorting polygons (only 2D)
* Optimizations (only 2D): Skip processing of invisible polygons, skip processing of duplicated points, normals

#### Requirements for 2D:
* Internet Explorer 9
* Chrome 4.0
* Firefox 2.0
* Safari 3.1, mobile Safari 3.2
* Opera 9.0, mobile Opera 10.0
* Android Browser 2.1

#### Requirements for WebGL:
* Chrome 9.0
* Firefox 4.0
* Safari 5.1 (needs to be enabled in Options)
* Opera 12.0

**Warning!** canvas-ply-reader.html and webgl-ply-reader.html won't work from disk because it uses AJAX to load **.ply** model file.

Performance for 2D
------------------

Intel Core2 Duo 2.00GHz

Suzanne monkey (500 polygons, 150-350 visible depending on side):
* Firefox 10.0: 34-68 fps
* Chromium 23: 65-95 fps

Utah teapot (2256 polygons, 1100 visible):
* Firefox 10.0: 7 fps
* Chromium 23: 13 fps

iPad 3: 1 GHz dual-core ARM Cortex-A9, iOS 6.0.1

Suzanne monkey (500 polygons, 150-350 visible depending on side):
* Safari: 13-23 fps

Utah teapot (2256 polygons, 1100 visible):
* Safari: 2 fps
