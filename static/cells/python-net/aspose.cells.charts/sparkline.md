##Sparkline class
## Sparkline class
A sparkline represents a tiny chart or graphic in a worksheet cell that provides a visual representation of data.
The Sparkline type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [data_range](/cells/python-net/aspose.cells.charts/sparkline/data_range) | Represents the data range of the sparkline. |
| [row](/cells/python-net/aspose.cells.charts/sparkline/row) | Gets the row index of the sparkline. |
| [column](/cells/python-net/aspose.cells.charts/sparkline/column) | Gets the column index of the sparkline. |
### Methods
| Method | Description |
| :- | :- |
| [`to_image(self, file_name, options)`](/cells/python-net/aspose.cells.charts/sparkline/to_image/#system.string-aspose.cells.rendering.imageorprintoptions) | Converts a sparkline to an image. |
| [`to_image(self, stream, options)`](/cells/python-net/aspose.cells.charts/sparkline/to_image/#io.rawiobase-aspose.cells.rendering.imageorprintoptions) | Converts a sparkline to an image. |
### Example
```python
from aspose.cells import CellArea, Workbook
from aspose.cells.charts import SparklineType
from aspose.cells.rendering import ImageOrPrintOptions
book = Workbook()
sheet = book.worksheets[0]
sheet.cells.get("A1").put_value(5)
sheet.cells.get("B1").put_value(2)
sheet.cells.get("C1").put_value(1)
sheet.cells.get("D1").put_value(3)
#  Define the CellArea
ca = CellArea()
ca.start_column = 4
ca.end_column = 4
ca.start_row = 0
ca.end_row = 0
idx = sheet.sparkline_groups.add(SparklineType.LINE, sheet.name + "!A1:D1", False, ca)
group = sheet.sparkline_groups[idx]
idx = group.sparklines.add(sheet.name + "!A1:D1", 0, 4)
line = group.sparklines[idx]
print("Saprkline data range: "  + line.data_range + ", row: "  + str(line.row) + ", column: "  + str(line.column))
line.to_image("output.png", ImageOrPrintOptions())
```
### See Also
* module [`aspose.cells.charts`](..)
