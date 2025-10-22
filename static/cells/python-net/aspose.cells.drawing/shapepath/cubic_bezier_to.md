##cubic_bezier_to method
## cubic_bezier_to(self, ctr_x1, ctr_y1, ctr_x2, ctr_y2, end_x, end_y) {#float-float-float-float-float-float}
Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure.Unit: Pixel.
```python
def cubic_bezier_to(self, ctr_x1, ctr_y1, ctr_x2, ctr_y2, end_x, end_y):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| ctr_x1 | float | The x-coordinate of the first control point for the curve(Unit: Pixel). |
| ctr_y1 | float | The y-coordinate of the first control point for the curve(Unit: Pixel). |
| ctr_x2 | float | The x-coordinate of the second control point for the curve(Unit: Pixel). |
| ctr_y2 | float | The y-coordinate of the second control point for the curve(Unit: Pixel). |
| end_x | float | The x-coordinate of the endpoint of the curve(Unit: Pixel). |
| end_y | float | The y-coordinate of the endpoint of the curve(Unit: Pixel). |
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`ShapePath`](/cells/python-net/aspose.cells.drawing/shapepath)
