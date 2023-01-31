---
title: Row class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 1300
url: /python-net/aspose.cells/row/
is_root: false
---

## Row class

Represents a single row in a worksheet.



The Row type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [is_blank](/cells/python-net/aspose.cells/row/is_blank) | Indicates whether the row contains any data |
| [is_collapsed](/cells/python-net/aspose.cells/row/is_collapsed) | whether the row is collapsed |
| [height](/cells/python-net/aspose.cells/row/height) | Gets and sets the row height in unit of Points. |
| [is_hidden](/cells/python-net/aspose.cells/row/is_hidden) | Indicates whether the row is hidden. |
| [index](/cells/python-net/aspose.cells/row/index) | Gets the index of this row. |
| [group_level](/cells/python-net/aspose.cells/row/group_level) | Gets the group level of the row. |
| [is_height_matched](/cells/python-net/aspose.cells/row/is_height_matched) | Indicates that row height and default font height matches. |
| [style](/cells/python-net/aspose.cells/row/style) | Represents the style of this row. |
| [has_custom_style](/cells/python-net/aspose.cells/row/has_custom_style) | Indicates whether this row has custom style settings(different from the default one inherited from workbook). |
| [first_cell](/cells/python-net/aspose.cells/row/first_cell) | Gets the first cell object in the row. |
| [first_data_cell](/cells/python-net/aspose.cells/row/first_data_cell) | Gets the first non-blank cell in the row. |
| [last_cell](/cells/python-net/aspose.cells/row/last_cell) | Gets the last cell object in the row. |
| [last_data_cell](/cells/python-net/aspose.cells/row/last_data_cell) | Gets the last non-blank cell in the row. |



Gets the cell.
### Indexer
| Name | Description |
| :- | :- |
| [index] | The column index |


### Methods
| Method | Description |
| :- | :- |
| [get_cell_by_index(index)](/cells/python-net/aspose.cells/row/get_cell_by_index/#int) | Get the cell by specific index in the list. |
| [get_cell_or_null(column)](/cells/python-net/aspose.cells/row/get_cell_or_null/#int) | Gets the cell or null in the specific index. |
| [get_style()](/cells/python-net/aspose.cells/row/get_style/#) | Gets the style of this row. |
| [set_style(style)](/cells/python-net/aspose.cells/row/set_style/#Style) | Sets the style of this row. |
| [copy_settings(source, check_style)](/cells/python-net/aspose.cells/row/copy_settings/#Row-bool) | Copy settings of row, such as style, height, visibility, ...etc. |
| [apply_style(style, flag)](/cells/python-net/aspose.cells/row/apply_style/#Style-StyleFlag) | Applies formats for a whole row. |
| [equals(row)](/cells/python-net/aspose.cells/row/equals/#Row) | Checks whether this object refers to the same row with another row object. |


### Example 


```
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()

# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
style = workbook.create_style()

# Setting the background color to Blue
style.background_color = Color.blue

# Setting the foreground color to Red
style.foreground_color = Color.red

# setting Background Pattern
style.pattern = BackgroundType.DIAGONAL_STRIPE

# New Style Flag
styleFlag = StyleFlag()

# Set All Styles
styleFlag.all = True

# Get first row
row = worksheet.cells.rows[0]

# Apply Style to first row
row.apply_style(style, styleFlag)

# Saving the Excel file
workbook.save("book1.xls")

```
### See Also

* module [aspose.cells](../)
