##HorizontalPageBreak class
## HorizontalPageBreak class
Encapsulates the object that represents a horizontal page break.
The HorizontalPageBreak type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [start_column](/cells/python-net/aspose.cells/horizontalpagebreak/start_column) | Gets the start column index of this horizontal page break. |
| [end_column](/cells/python-net/aspose.cells/horizontalpagebreak/end_column) | Gets the end column index of this horizontal page break. |
| [row](/cells/python-net/aspose.cells/horizontalpagebreak/row) | Gets the zero based row index. |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Add a page break at cell Y30
Index = worksheet.horizontal_page_breaks.add("Y30")
# get the newly added horizontal page break
hPageBreak = worksheet.horizontal_page_breaks[Index]
```
### See Also
* module [`aspose.cells`](..)
