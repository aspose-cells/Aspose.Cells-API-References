##ShapePath class
## ShapePath class
Represents a creation path consisting of a series of moves, lines and curves that when combined will form a geometric shape.
The ShapePath type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells.drawing/shapepath/__init__/#) | Initializes a new instance of the [`ShapePath`](/cells/python-net/aspose.cells.drawing/shapepath) class. |
### Properties
| Property | Description |
| :- | :- |
| [path_segement_list](/cells/python-net/aspose.cells.drawing/shapepath/path_segement_list) | Gets [`ShapeSegmentPathCollection`](/cells/python-net/aspose.cells.drawing/shapesegmentpathcollection) list |
| [width_pixel](/cells/python-net/aspose.cells.drawing/shapepath/width_pixel) | Gets the width of this path in unit of pixels. |
| [height_pixel](/cells/python-net/aspose.cells.drawing/shapepath/height_pixel) | Gets the height of this path in unit of pixels. |
### Methods
| Method | Description |
| :- | :- |
| [`move_to(self, x, y)`](/cells/python-net/aspose.cells.drawing/shapepath/move_to/#float-float) | Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure.Unit: Pixel. |
| [`line_to(self, x, y)`](/cells/python-net/aspose.cells.drawing/shapepath/line_to/#float-float) | Appends a line segment to the current figure.
| [`cubic_bezier_to(self, ctr_x1, ctr_y1, ctr_x2, ctr_y2, end_x, end_y)`](/cells/python-net/aspose.cells.drawing/shapepath/cubic_bezier_to/#float-float-float-float-float-float) | Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure.Unit: Pixel. |
| [`arc_to(self, w_r, h_r, st_ang, sw_ang)`](/cells/python-net/aspose.cells.drawing/shapepath/arc_to/#float-float-float-float) | Appends an elliptical arc to the current figure. The starting point is the end point of the current figure. |
| [`close(self)`](/cells/python-net/aspose.cells.drawing/shapepath/close/#) | Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves, the method closes the loop by connecting a line from the endpoint to the starting point. |
### See Also
* module [`aspose.cells.drawing`](..)
* class [`ShapePath`](/cells/python-net/aspose.cells.drawing/shapepath)
* class [`ShapeSegmentPathCollection`](/cells/python-net/aspose.cells.drawing/shapesegmentpathcollection)
