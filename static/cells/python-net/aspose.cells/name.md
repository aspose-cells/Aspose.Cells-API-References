##Name class
## Name class
Represents a defined name for a range of cells.
The Name type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [comment](/cells/python-net/aspose.cells/name/comment) | Gets and sets the comment of the name.
| [text](/cells/python-net/aspose.cells/name/text) | Gets the name text of the object. |
| [full_text](/cells/python-net/aspose.cells/name/full_text) | Gets the name  full text of the object with the scope setting. |
| [refers_to](/cells/python-net/aspose.cells/name/refers_to) | Returns or sets the formula that the name is defined to refer to, beginning with an equal sign. |
| [r1c1_refers_to](/cells/python-net/aspose.cells/name/r1c1_refers_to) | Gets or sets a R1C1 reference of the [`Name`](/cells/python-net/aspose.cells/name). |
| [is_referred](/cells/python-net/aspose.cells/name/is_referred) | Indicates whether this name is referred by other formulas. |
| [is_visible](/cells/python-net/aspose.cells/name/is_visible) | Indicates whether the name is visible. |
| [sheet_index](/cells/python-net/aspose.cells/name/sheet_index) | Indicates this name belongs to Workbook or Worksheet.
### Methods
| Method | Description |
| :- | :- |
| [`get_refers_to(self, is_r1c1, is_local)`](/cells/python-net/aspose.cells/name/get_refers_to/#bool-bool) | Get the reference of this Name. |
| [`get_refers_to(self, is_r1c1, is_local, row, column)`](/cells/python-net/aspose.cells/name/get_refers_to/#bool-bool-int-int) | Get the reference of this Name based on specified cell. |
| [`get_ranges(self)`](/cells/python-net/aspose.cells/name/get_ranges/#) | Gets all ranges referred by this name. |
| [`get_ranges(self, recalculate)`](/cells/python-net/aspose.cells/name/get_ranges/#bool) | Gets all ranges referred by this name. |
| [`get_range(self)`](/cells/python-net/aspose.cells/name/get_range/#) | Gets the range if this name refers to a range. |
| [`get_range(self, recalculate)`](/cells/python-net/aspose.cells/name/get_range/#bool) | Gets the range if this name refers to a range |
| [`get_range(self, sheet_index, row, column)`](/cells/python-net/aspose.cells/name/get_range/#int-int-int) | Gets the range if this name refers to a range.
| [`set_refers_to(self, refers_to, is_r1c1, is_local)`](/cells/python-net/aspose.cells/name/set_refers_to/#system.string-bool-bool) | Set the reference of this Name. |
| [`get_referred_areas(self, recalculate)`](/cells/python-net/aspose.cells/name/get_referred_areas/#bool) | Gets all references referred by this name. |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating a named range
range = worksheet.cells.create_range("B4", "G14")
# Setting the name of the named range
range.name = "TestRange"
# Saving the modified Excel file in default (that is Excel 2000) format
workbook.save("output.xls")
```
### See Also
* module [`aspose.cells`](..)
* class [`Name`](/cells/python-net/aspose.cells/name)
