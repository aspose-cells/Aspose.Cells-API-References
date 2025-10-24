##auto_fill method
## auto_fill(self, target) {#aspose.cells.Range}
Automaticall fill the target range.
```python
def auto_fill(self, target):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| target | aspose.cells.Range | the target range. |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
cells.get("A1").put_value(1)
cells.get("A2").put_value(2)
source = cells.create_range("A1:A2")
target = cells.create_range("A3:A10")
# fill 3,4,5....10 to the range A3:A10
source.auto_fill(target)
# Save the Excel file
workbook.save("book1.xlsm")
```
## auto_fill(self, target, auto_fill_type) {#aspose.cells.Range-aspose.cells.AutoFillType}
Automaticall fill the target range.
```python
def auto_fill(self, target, auto_fill_type):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| target | aspose.cells.Range | The targed range. |
| auto_fill_type | aspose.cells.AutoFillType | The auto fill type. |
### See Also
* module [`aspose.cells`](../../)
* class [`Range`](/cells/python-net/aspose.cells/range)
