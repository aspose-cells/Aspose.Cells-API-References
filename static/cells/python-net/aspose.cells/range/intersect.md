##intersect method
## intersect(self, range) {#aspose.cells.Range}
Returns a [`Range`](/cells/python-net/aspose.cells/range) object that represents the rectangular intersection of two ranges.
### Returns
Returns a [`Range`](/cells/python-net/aspose.cells/range) object
```python
def intersect(self, range):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| range | aspose.cells.Range | The intersecting range. |
### Remarks
If the two ranges are not intersected, returns null.
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
range1 = cells.create_range("A1:A5")
range2 = cells.create_range("A3:A10")
# Get intersected range of the two ranges.
intersectRange = range1.intersect(range2)
# Save the Excel file
workbook.save("book1.xlsm")
```
### See Also
* module [`aspose.cells`](../../)
* class [`Range`](/cells/python-net/aspose.cells/range)
