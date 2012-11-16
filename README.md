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
* Painter''s algorithm for sorting polygons
* Optimizations: Skip processing of invisible polygons, skip processing of duplicated points, normals


#### Requirements:
* Internet Explorer 9
* Firefox 2.0
* Safari 3.1
* Opera 9.0
* Safari (Mobile) 3.2
* Opera (Mobile) 10.0
* Android Browser 2.1

**Warning!** canvas-ply-reader.html won''t work from disk because it uses AJAX to load **.ply** model file.
