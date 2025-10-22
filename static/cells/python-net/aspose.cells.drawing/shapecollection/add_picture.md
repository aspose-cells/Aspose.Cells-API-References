##add_picture method
## add_picture(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream) {#int-int-int-int-io.RawIOBase}
Adds a picture to the collection.
### Returns
[`Picture`](/cells/python-net/aspose.cells.drawing/picture) Picture object.
```python
def add_picture(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| upper_left_column | int | Upper left column index. |
| lower_right_row | int | Lower right row index |
| lower_right_column | int | Lower right column index |
| stream | io.RawIOBase | Stream object which contains the image data. |
### Example
```python
# add a picture
with open("image.jpg", "rb") as fs:
picture = shapes.add_picture(1, 0, 1, 0, fs)
```
## add_picture(self, upper_left_row, upper_left_column, stream, width_scale, height_scale) {#int-int-io.RawIOBase-int-int}
Adds a picture to the collection.
### Returns
[`Picture`](/cells/python-net/aspose.cells.drawing/picture) Picture object.
```python
def add_picture(self, upper_left_row, upper_left_column, stream, width_scale, height_scale):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| upper_left_column | int | Upper left column index. |
| stream | io.RawIOBase | Stream object which contains the image data. |
| width_scale | int | Scale of image width, a percentage. |
| height_scale | int | Scale of image height, a percentage. |
### Example
```python
# add a picture
with open("image.jpg", "rb") as fs:
picture = shapes.add_picture(1, 1, fs, 50, 60)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Picture`](/cells/python-net/aspose.cells.drawing/picture)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
