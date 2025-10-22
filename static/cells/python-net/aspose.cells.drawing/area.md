##Area class
## Area class
Encapsulates the object that represents an area format.
The Area type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [background_color](/cells/python-net/aspose.cells.drawing/area/background_color) | Gets or sets the background Color of the [`Area`](/cells/python-net/aspose.cells.drawing/area). |
| [foreground_color](/cells/python-net/aspose.cells.drawing/area/foreground_color) | Gets or sets the foreground Color. |
| [formatting](/cells/python-net/aspose.cells.drawing/area/formatting) | Represents the formatting of the area. |
| [invert_if_negative](/cells/python-net/aspose.cells.drawing/area/invert_if_negative) | If the property is true and the value of chart point is a negative number,
| [fill_format](/cells/python-net/aspose.cells.drawing/area/fill_format) | Represents a [`Area.fill_format`](/cells/python-net/aspose.cells.drawing/area#fill_format) object that contains fill formatting properties for the specified chart or shape. |
| [transparency](/cells/python-net/aspose.cells.drawing/area/transparency) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
### Example
```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.pydrawing import Color
# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Workbook object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Setting the foreground color of the plot area
chart.plot_area.area.foreground_color = Color.blue
# Setting the foreground color of the chart area
chart.chart_area.area.foreground_color = Color.yellow
# Setting the foreground color of the 1st NSeries area
chart.n_series[0].area.foreground_color = Color.red
# Setting the foreground color of the area of the 1st NSeries point
chart.n_series[0].points[0].area.foreground_color = Color.cyan
# Saving the Excel file
workbook.save("book1.xls")
```
### See Also
* module [`aspose.cells.drawing`](..)
* class [`Area`](/cells/python-net/aspose.cells.drawing/area)
