##add_picture_in_chart method
## add_picture_in_chart(self, top, left, stream, width_scale, height_scale) {#int-int-io.RawIOBase-int-int}
Adds a picture to the chart.
### Returns
Returns a Picture object.
```python
def add_picture_in_chart(self, top, left, stream, width_scale, height_scale):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| top | int | Represents the vertical offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| left | int | Represents the horizontal offset of shape from the upper left corner in units of 1/4000 of the chart area. |
| stream | io.RawIOBase | Stream object which contains the image data. |
| width_scale | int | Scale of image width, a percentage. |
| height_scale | int | Scale of image height, a percentage. |
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Picture`](/cells/python-net/aspose.cells.drawing/picture)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
