##horizontal_resolution property
## horizontal_resolution property
Gets or sets the horizontal resolution for generated images, in dots per inch.
### Remarks
The default value is 96.
Setting [`ImageOrPrintOptions.horizontal_resolution`](/cells/python-net/aspose.cells.rendering/imageorprintoptions#horizontal_resolution) and [`ImageOrPrintOptions.vertical_resolution`](/cells/python-net/aspose.cells.rendering/imageorprintoptions#vertical_resolution)
effects the width and height of the output image in pixels.
### Example
The following code sets resolution to 192, the width and height of the generated image is twice of
the one with resolution left as the default value 96.
```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender
wb = Workbook("Book1.xlsx")
opts = ImageOrPrintOptions()
# Set output image type: png.
opts.image_type = ImageType.PNG
# Set resolution to 192.
opts.horizontal_resolution = 192
opts.vertical_resolution = 192
# Render worksheet page to image.
sr = SheetRender(wb.worksheets[0], opts)
sr.to_image(0, "Sheet_Page1.png")
```
### Definition:
```python
@property
def horizontal_resolution(self):
...
@horizontal_resolution.setter
def horizontal_resolution(self, value):
...
```
### See Also
* module [`aspose.cells.rendering`](../../)
* class [`ImageOrPrintOptions`](/cells/python-net/aspose.cells.rendering/imageorprintoptions)
