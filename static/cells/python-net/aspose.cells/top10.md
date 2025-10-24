##Top10 class
## Top10 class
Describe the Top10 conditional formatting rule.
This conditional formatting rule highlights cells whose
values fall in the top N or bottom N bracket, as specified.
The Top10 type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/top10/__init__/#) | Constructs a new instance of Top10 |
### Properties
| Property | Description |
| :- | :- |
| [is_percent](/cells/python-net/aspose.cells/top10/is_percent) | Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule.
| [is_bottom](/cells/python-net/aspose.cells/top10/is_bottom) | Get or set whether a "top/bottom n" rule is a "bottom n" rule.
| [rank](/cells/python-net/aspose.cells/top10/rank) | Get or set the value of "n" in a "top/bottom n" conditional formatting rule.
### Example
```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color
# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea.create_cell_area(0, 0, 10, 10)
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.TOP10, OperatorType.NONE, None, None)
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
top10 = fc.top10
# Set the Top N
top10.rank = 5
# Saving the Excel file
workbook.save("output.xls")
```
### See Also
* module [`aspose.cells`](..)
