##DataBar class
## DataBar class
Describe the DataBar conditional formatting rule.
This conditional formatting rule displays a gradated
data bar in the range of cells.
The DataBar type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [axis_color](/cells/python-net/aspose.cells/databar/axis_color) | Gets the color of the axis for cells with conditional formatting as data bars. |
| [axis_position](/cells/python-net/aspose.cells/databar/axis_position) | Gets or sets the position of the axis of the data bars specified by a conditional formatting rule. |
| [bar_fill_type](/cells/python-net/aspose.cells/databar/bar_fill_type) | Gets or sets how a data bar is filled with color. |
| [direction](/cells/python-net/aspose.cells/databar/direction) | Gets or sets the direction the databar is displayed. |
| [bar_border](/cells/python-net/aspose.cells/databar/bar_border) | Gets an object that specifies the border of a data bar. |
| [negative_bar_format](/cells/python-net/aspose.cells/databar/negative_bar_format) | Gets the NegativeBarFormat object associated with a data bar conditional formatting rule. |
| [min_cfvo](/cells/python-net/aspose.cells/databar/min_cfvo) | Get or set this DataBar's min value object.
| [max_cfvo](/cells/python-net/aspose.cells/databar/max_cfvo) | Get or set this DataBar's max value object.
| [color](/cells/python-net/aspose.cells/databar/color) | Get or set this DataBar's Color. |
| [min_length](/cells/python-net/aspose.cells/databar/min_length) | Represents the min length of data bar . |
| [max_length](/cells/python-net/aspose.cells/databar/max_length) | Represents the max length of data bar . |
| [show_value](/cells/python-net/aspose.cells/databar/show_value) | Get or set the flag indicating whether to show the values of the cells on which this data bar is applied.
### Methods
| Method | Description |
| :- | :- |
| [`to_image(self, cell, img_opts)`](/cells/python-net/aspose.cells/databar/to_image/#aspose.cells.cell-aspose.cells.rendering.imageorprintoptions) | Render data bar in cell to image byte array. |
### Example
```python
from aspose.cells import CellArea, DataBarAxisPosition, DataBarBorderType, DataBarFillType, DataBarNegativeColorType, FormatConditionType, FormatConditionValueType, Workbook
from aspose.pydrawing import Color
# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 2
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
# Adds condition.
idx = fcs.add_condition(FormatConditionType.DATA_BAR)
fcs.add_area(ca)
cond = fcs[idx]
# Get Databar
dataBar = cond.data_bar
dataBar.color = Color.orange
# Set Databar properties
dataBar.min_cfvo.type = FormatConditionValueType.PERCENTILE
dataBar.min_cfvo.value = 30
dataBar.show_value = False
dataBar.bar_border.type = DataBarBorderType.SOLID
dataBar.bar_border.color = Color.plum
dataBar.bar_fill_type = DataBarFillType.SOLID
dataBar.axis_color = Color.red
dataBar.axis_position = DataBarAxisPosition.MIDPOINT
dataBar.negative_bar_format.color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.color = Color.white
dataBar.negative_bar_format.border_color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.border_color = Color.yellow
# Put Cell Values
cell1 = sheet.cells.get("A1")
cell1.put_value(10)
cell2 = sheet.cells.get("A2")
cell2.put_value(120)
cell3 = sheet.cells.get("A3")
cell3.put_value(260)
# Saving the Excel file
workbook.save("book1.xlsx")
```
### See Also
* module [`aspose.cells`](..)
