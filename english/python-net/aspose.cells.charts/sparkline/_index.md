---
title: Sparkline class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 260
url: /python-net/aspose.cells.charts/sparkline/
is_root: false
---

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
| [to_image(file_name, options)](/cells/python-net/aspose.cells.charts/sparkline/to_image/#str-aspose.cells.rendering.ImageOrPrintOptions) | Converts a sparkline to an image. |
| [to_image(stream, options)](/cells/python-net/aspose.cells.charts/sparkline/to_image/#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions) | Converts a sparkline to an image. |



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
idx = sheet.sparkline_group_collection.add(SparklineType.LINE, sheet.name + "!A1:D1", False, ca)
group = sheet.sparkline_group_collection[idx]
idx = group.sparkline_collection.add(sheet.name + "!A1:D1", 0, 4)
line = group.sparkline_collection[idx]
print("Saprkline data range: "  + line.data_range + ", row: "  + str(line.row) + ", column: "  + str(line.column))
line.to_image("output.png", ImageOrPrintOptions())

```

### See Also
* module [aspose.cells.charts](..)
