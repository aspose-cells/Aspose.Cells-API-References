##Column class
## Column class
Represents a single column in a worksheet.
The Column type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [index](/cells/python-net/aspose.cells/column/index) | Gets the index of this column. |
| [width](/cells/python-net/aspose.cells/column/width) | Gets and sets the column width in unit of characters. |
| [group_level](/cells/python-net/aspose.cells/column/group_level) | Gets the group level of the column. |
| [is_hidden](/cells/python-net/aspose.cells/column/is_hidden) | Indicates whether the column is hidden. |
| [has_custom_style](/cells/python-net/aspose.cells/column/has_custom_style) | Indicates whether this column has custom style settings(different from the default one inherited from workbook). |
| [style](/cells/python-net/aspose.cells/column/style) | Gets the style of this column. |
| [is_collapsed](/cells/python-net/aspose.cells/column/is_collapsed) | whether the column is collapsed |
### Methods
| Method | Description |
| :- | :- |
| [`apply_style(self, style, flag)`](/cells/python-net/aspose.cells/column/apply_style/#aspose.cells.style-aspose.cells.styleflag) | Applies formats for a whole column. |
| [`get_style(self)`](/cells/python-net/aspose.cells/column/get_style/#) | Gets the style of this column. |
| [`set_style(self, style)`](/cells/python-net/aspose.cells/column/set_style/#aspose.cells.style) | Sets the style of this column. |
### Example
```python
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
# Get first Column
column = worksheet.cells.columns[0]
# Apply Style to first Column
column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")
```
### See Also
* module [`aspose.cells`](..)
