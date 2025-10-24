##FindOptions class
## FindOptions class
Represents find options.
The FindOptions type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/findoptions/__init__/#) | Constructs a new instance of FindOptions |
### Properties
| Property | Description |
| :- | :- |
| [is_case_sensitive](/cells/python-net/aspose.cells/findoptions/is_case_sensitive) | Indicates if the searched string is case sensitive. |
| [case_sensitive](/cells/python-net/aspose.cells/findoptions/case_sensitive) | Indicates if the searched string is case sensitive. |
| [look_at_type](/cells/python-net/aspose.cells/findoptions/look_at_type) | Look at type. |
| [is_range_set](/cells/python-net/aspose.cells/findoptions/is_range_set) | Indicates whether the searched range is set. |
| [search_next](/cells/python-net/aspose.cells/findoptions/search_next) | Search order. True: search next. False: search previous. |
| [search_backward](/cells/python-net/aspose.cells/findoptions/search_backward) | Whether search backward for cells. |
| [seach_order_by_rows](/cells/python-net/aspose.cells/findoptions/seach_order_by_rows) | Indicates whether search order by rows or columns. |
| [search_order_by_rows](/cells/python-net/aspose.cells/findoptions/search_order_by_rows) | Indicates whether search order by rows or columns. |
| [look_in_type](/cells/python-net/aspose.cells/findoptions/look_in_type) | Look in type. |
| [regex_key](/cells/python-net/aspose.cells/findoptions/regex_key) | Indicates whether the searched key is regex.
| [value_type_sensitive](/cells/python-net/aspose.cells/findoptions/value_type_sensitive) | Indicates whether searched cell value type should be same with the searched key. |
| [style](/cells/python-net/aspose.cells/findoptions/style) | The format to search for. |
| [convert_numeric_data](/cells/python-net/aspose.cells/findoptions/convert_numeric_data) | Gets or sets a value that indicates whether converting the searched string value to numeric data. |
### Methods
| Method | Description |
| :- | :- |
| [`get_range(self)`](/cells/python-net/aspose.cells/findoptions/get_range/#) | Gets and sets the searched range. |
| [`set_range(self, ca)`](/cells/python-net/aspose.cells/findoptions/set_range/#aspose.cells.cellarea) | Sets the searched range. |
### Example
```python
from aspose.cells import CellArea, FindOptions, LookInType, Workbook
# Instantiate the workbook object
workbook = Workbook("book1.xls")
# Get Cells collection
cells = workbook.worksheets[0].cells
# Instantiate FindOptions Object
findOptions = FindOptions()
# Create a Cells Area
ca = CellArea()
ca.start_row = 8
ca.start_column = 2
ca.end_row = 17
ca.end_column = 13
# Set cells area for find options
findOptions.set_range(ca)
# Set searching properties
findOptions.search_backward = False
findOptions.seach_order_by_rows = True
findOptions.look_in_type = LookInType.VALUES
# Find the cell with 0 value
cell = cells.find(0, None, findOptions)
```
### See Also
* module [`aspose.cells`](..)
