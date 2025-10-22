##copy method
## copy(self, range) {#aspose.cells.Range}
Copies data (including formulas), formatting, drawing objects etc. from a source range.
```python
def copy(self, range):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| range | aspose.cells.Range | Source [`Range`](/cells/python-net/aspose.cells/range) object. |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
range1 = cells.create_range("A1:A5")
range2 = cells.create_range("A6:A10")
# Copy the range.
range1.copy(range2)
# Save the Excel file
workbook.save("book1.xlsm")
```
## copy(self, range, options) {#aspose.cells.Range-aspose.cells.PasteOptions}
Copying the range with paste special options.
```python
def copy(self, range, options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| range | aspose.cells.Range | The source range. |
| options | aspose.cells.PasteOptions | The paste special options. |
### See Also
* module [`aspose.cells`](../../)
* class [`Range`](/cells/python-net/aspose.cells/range)
