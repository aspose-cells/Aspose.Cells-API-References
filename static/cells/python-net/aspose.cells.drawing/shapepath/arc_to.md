##arc_to method
## arc_to(self, w_r, h_r, st_ang, sw_ang) {#float-float-float-float}
Appends an elliptical arc to the current figure. The starting point is the end point of the current figure.
```python
def arc_to(self, w_r, h_r, st_ang, sw_ang):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| w_r | float | The half-width of the rectangular area of ​​the ellipse that draws the arc(Unit: Pixel). |
| h_r | float | The half-height of the rectangular area of ​​the ellipse that draws the arc(Unit: Pixel). |
| st_ang | float | The starting angle of the arc, measured in degrees clockwise from the x-axis(Unit: Degree). This angle will specify what angle along the supposed circle path will be used as the start position for drawing the arc. This start angle will be locked to the last known pen position in the shape path. Thus guaranteeing a continuos shape path. |
| sw_ang | float | The swing angle for an arc. This angle will specify how far angle-wise along the supposed cicle path the arc will be extended. The extension from the start angle will always be in the clockwise direction around the supposed circle.(Unit: Degree) |
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`ShapePath`](/cells/python-net/aspose.cells.drawing/shapepath)
