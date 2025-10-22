##add method
## add(self, upper_left_row, upper_left_column, stream) {#int-int-io.RawIOBase}
Adds a picture to the collection.
### Returns
[`Picture`](/cells/python-net/aspose.cells.drawing/picture) object index.
```python
def add(self, upper_left_row, upper_left_column, stream):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| upper_left_column | int | Upper left column index. |
| stream | io.RawIOBase | Stream object which contains the image data. |
### Example
```python
# add a picture
with open("image.jpg", "rb") as fs:
pictures.add(1, 1, fs)
```
## add(self, upper_left_row, upper_left_column, file_name) {#int-int-System.String}
Adds a picture to the collection.
### Returns
[`Picture`](/cells/python-net/aspose.cells.drawing/picture) object index.
```python
def add(self, upper_left_row, upper_left_column, file_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| upper_left_column | int | Upper left column index. |
| file_name | System.String | Image filename. |
### Example
```python
# add a picture
pictures.add(1, 1, "image.jpg")
```
## add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream) {#int-int-int-int-io.RawIOBase}
Adds a picture to the collection.
### Returns
[`Picture`](/cells/python-net/aspose.cells.drawing/picture) object index.
```python
def add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream):
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
pictures.add(1, 1, 5, 5, fs)
```
## add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name) {#int-int-int-int-System.String}
Adds a picture to the collection.
### Returns
[`Picture`](/cells/python-net/aspose.cells.drawing/picture) object index.
```python
def add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| upper_left_column | int | Upper left column index. |
| lower_right_row | int | Lower right row index |
| lower_right_column | int | Lower right column index |
| file_name | System.String | Image filename. |
### Example
```python
# add a picture
pictures.add(1, 1, 5, 5, "image.jpg")
```
## add(self, upper_left_row, upper_left_column, stream, width_scale, height_scale) {#int-int-io.RawIOBase-int-int}
Adds a picture to the collection.
### Returns
[`Picture`](/cells/python-net/aspose.cells.drawing/picture) object index.
```python
def add(self, upper_left_row, upper_left_column, stream, width_scale, height_scale):
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
pictures.add(1, 1, fs, 50, 50)
```
## add(self, upper_left_row, upper_left_column, file_name, width_scale, height_scale) {#int-int-System.String-int-int}
Adds a picture to the collection.
### Returns
[`Picture`](/cells/python-net/aspose.cells.drawing/picture) object index.
```python
def add(self, upper_left_row, upper_left_column, file_name, width_scale, height_scale):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| upper_left_column | int | Upper left column index. |
| file_name | System.String | Image filename. |
| width_scale | int | Scale of image width, a percentage. |
| height_scale | int | Scale of image height, a percentage. |
### Example
```python
# add a picture
pictures.add(1, 1, "image.jpg", 50, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Picture`](/cells/python-net/aspose.cells.drawing/picture)
* class [`PictureCollection`](/cells/python-net/aspose.cells.drawing/picturecollection)
