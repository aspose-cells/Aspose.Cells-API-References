##set_desired_size method
## set_desired_size(self, desired_width, desired_height) {#int-int}
Sets desired width and height of image.
```python
def set_desired_size(self, desired_width, desired_height):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| desired_width | int | desired width in pixels |
| desired_height | int | desired height in pixels |
### Remarks
NOTE: This member is now obsolete. Instead,
please use [`ImageOrPrintOptions.set_desired_size`](/cells/python-net/aspose.cells.rendering/imageorprintoptions/set_desired_size) by setting param keepAspectRatio to false.
This property will be removed 12 months later since May 2023.
Aspose apologizes for any inconvenience you may have experienced.
## set_desired_size(self, desired_width, desired_height, keep_aspect_ratio) {#int-int-bool}
Sets desired width and height of image.
```python
def set_desired_size(self, desired_width, desired_height, keep_aspect_ratio):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| desired_width | int | desired width in pixels |
| desired_height | int | desired height in pixels |
| keep_aspect_ratio | bool | whether to keep aspect ratio of origin image |
### Remarks
The width and height of the output image in pixels will be only based on
the set desired width and height.
The [`ImageOrPrintOptions.horizontal_resolution`](/cells/python-net/aspose.cells.rendering/imageorprintoptions#horizontal_resolution) and [`ImageOrPrintOptions.vertical_resolution`](/cells/python-net/aspose.cells.rendering/imageorprintoptions#vertical_resolution)
will not effect the width and height of the output image in this case.
### See Also
* module [`aspose.cells.rendering`](../../)
* class [`SvgImageOptions`](/cells/python-net/aspose.cells.rendering/svgimageoptions)
