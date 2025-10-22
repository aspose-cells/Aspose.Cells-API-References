##border_weight property
## border_weight property
Gets or sets the weight of the border line of a picture in units of pt.
### Example
```python
from aspose.cells import Workbook
from aspose.pydrawing import Color
# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
imgIndex = worksheet.pictures.add(1, 1, "example.jpeg")
# Get the inserted picture object
pic = worksheet.pictures[imgIndex]
# Set the border color of the picture
pic.border_line_color = Color.red
# Set the border width of the picture
pic.border_weight = 3.0
# Save the excel file.
workbook.save("result.xlsx")
```
### Definition:
```python
@property
def border_weight(self):
...
@border_weight.setter
def border_weight(self, value):
...
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Picture`](/cells/python-net/aspose.cells.drawing/picture)
