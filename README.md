PLY 3D model viewer based on HTML5 canvas
=========================================

3D HTML5 canvas realization based on 2D context.

Examples:
* [Cube](http://gnomeby.github.com/canvas3D/canvas-3d-cube.html) (see **Cube function** in source code)
* [Suzanne monkey](http://gnomeby.github.com/canvas3D/canvas-ply-reader.html?file=monkey.ply)
* [Utah teapot](http://gnomeby.github.com/canvas3D/canvas-ply-reader.html?file=teapot.ply)


Features:
* 3D operations: rotating, moving object center
* Direct illumination
* Highlighting edges
* Painter's algorithm for sorting polygons
* Optimizations: Skip processing of invisible polygons, skip processing of duplicated points, normals


#### Requirements:
* Internet Explorer 9
* Chrome 4.0
* Firefox 2.0
* Safari 3.1, mobile Safari 3.2
* Opera 9.0, mobile Opera 10.0
* Android Browser 2.1

**Warning!** canvas-ply-reader.html won't work from disk because it uses AJAX to load **.ply** model file.

Performance
-----------

Intel Core2 Duo 2.00GHz

Suzanne monkey (500 polygons):
* Firefox 10.0: 34-68 fps
* Chromium 23: 65-95 fps

Utah teapot (2256 polygons):
* Firefox 10.0: 7 fps
* Chromium 23: 13 fps
