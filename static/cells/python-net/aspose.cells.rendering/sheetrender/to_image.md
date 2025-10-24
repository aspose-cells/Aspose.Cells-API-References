##to_image method
## to_image(self, page_index, file_name) {#int-System.String}
Render certain page to a file.
```python
def to_image(self, page_index, file_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | indicate which page is to be converted |
| file_name | System.String | filename of the output image |
### Example
The following code outputs the first page of the first sheet to png image.
```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender
# load the source file with images.
wb = Workbook("Book1.xlsx")
imgOpt = ImageOrPrintOptions()
# set output image type.
imgOpt.image_type = ImageType.PNG
# render the first sheet.
sr = SheetRender(wb.worksheets[0], imgOpt)
# output the first page of the sheet to image.
sr.to_image(0, "output.png")
```
## to_image(self, page_index, stream) {#int-io.RawIOBase}
Render certain page to a stream.
```python
def to_image(self, page_index, stream):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| page_index | int | indicate which page is to be converted |
| stream | io.RawIOBase | the stream of the output image |
### See Also
* module [`aspose.cells.rendering`](../../)
* class [`SheetRender`](/cells/python-net/aspose.cells.rendering/sheetrender)
