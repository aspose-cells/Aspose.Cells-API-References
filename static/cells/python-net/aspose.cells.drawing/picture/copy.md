##copy method
## copy(self, source, options) {#aspose.cells.drawing.Picture-aspose.cells.CopyOptions}
Copy the picture.
```python
def copy(self, source, options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| source | aspose.cells.drawing.Picture | The source picture. |
| options | aspose.cells.CopyOptions | The copy options. |
### Example
```python
from aspose.cells import CopyOptions, Workbook
# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# insert first picture
imgIndex1 = worksheet.pictures.add(1, 1, "1.png")
# Get the inserted picture object
pic1 = worksheet.pictures[imgIndex1]
# insert second picture
imgIndex2 = worksheet.pictures.add(1, 9, "2.jpeg")
# Get the inserted picture object
pic2 = worksheet.pictures[imgIndex2]
# Copy picture 1 to picture 2.You'll get two picture 1 objects that are superimposed on top of each other.
opt = CopyOptions()
pic2.copy(pic1, opt)
# Save the excel file.
workbook.save("result.xlsx")
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Picture`](/cells/python-net/aspose.cells.drawing/picture)
