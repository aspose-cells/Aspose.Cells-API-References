##characters method
## characters(self, start_index, length) {#int-int}
Returns a Characters object that represents a range of characters within the cell text.
### Returns
Characters object.
```python
def characters(self, start_index, length):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| start_index | int | The index of the start of the character. |
| length | int | The number of characters. |
### Remarks
This method only works on cell with string value.
### Example
```python
from aspose.cells import Workbook
from aspose.pydrawing import Color
excel = Workbook()
cells = excel.worksheets[0].cells
cells.get("A1").put_value("Helloworld")
cells.get("A1").characters(5, 5).font.is_bold = True
cells.get("A1").characters(5, 5).font.color = Color.blue
```
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
* class [`FontSetting`](/cells/python-net/aspose.cells/fontsetting)
