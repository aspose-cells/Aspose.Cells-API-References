##VerticalPageBreak class
## VerticalPageBreak class
Encapsulates the object that represents a vertical page break.
The VerticalPageBreak type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [start_row](/cells/python-net/aspose.cells/verticalpagebreak/start_row) | Gets the start row index of the vertical page break. |
| [end_row](/cells/python-net/aspose.cells/verticalpagebreak/end_row) | Gets the end row index of the vertical page break. |
| [column](/cells/python-net/aspose.cells/verticalpagebreak/column) | Gets the column index of the vertical page break. |
### Example
```python
from aspose.cells import Workbook
excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")
```
### See Also
* module [`aspose.cells`](..)
