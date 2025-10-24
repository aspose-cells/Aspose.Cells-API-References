##formula property
## formula property
Gets or sets a formula of the [`Cell`](/cells/python-net/aspose.cells/cell).
### Remarks
A formula string always begins with an equal sign (=).
And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)".
### Example
```python
from aspose.cells import Workbook
excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("B6").formula = "=SUM(B2:B5, E1) + sheet1!A1"
```
### Definition:
```python
@property
def formula(self):
...
@formula.setter
def formula(self, value):
...
```
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
