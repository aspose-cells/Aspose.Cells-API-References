##ChartDataTable class
## ChartDataTable class
Represents a chart data table.
The ChartDataTable type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [font](/cells/python-net/aspose.cells.charts/chartdatatable/font) | Gets a [`ChartDataTable.font`](/cells/python-net/aspose.cells.charts/chartdatatable#font) object which represents the font setting of the specified chart data table. |
| [auto_scale_font](/cells/python-net/aspose.cells.charts/chartdatatable/auto_scale_font) | True if the text in the object changes font size when the object size changes.
| [background_mode](/cells/python-net/aspose.cells.charts/chartdatatable/background_mode) | Gets and sets the display mode of the background |
| [has_border_horizontal](/cells/python-net/aspose.cells.charts/chartdatatable/has_border_horizontal) | True if the chart data table has horizontal cell borders |
| [has_horizontal_border](/cells/python-net/aspose.cells.charts/chartdatatable/has_horizontal_border) | True if the chart data table has horizontal cell borders |
| [has_border_vertical](/cells/python-net/aspose.cells.charts/chartdatatable/has_border_vertical) | True if the chart data table has vertical cell borders |
| [has_vertical_border](/cells/python-net/aspose.cells.charts/chartdatatable/has_vertical_border) | True if the chart data table has vertical cell borders |
| [has_border_outline](/cells/python-net/aspose.cells.charts/chartdatatable/has_border_outline) | True if the chart data table has outline borders |
| [has_outline_border](/cells/python-net/aspose.cells.charts/chartdatatable/has_outline_border) | True if the chart data table has outline borders |
| [show_legend_key](/cells/python-net/aspose.cells.charts/chartdatatable/show_legend_key) | True if the data label legend key is visible. |
| [border](/cells/python-net/aspose.cells.charts/chartdatatable/border) | Returns a Border object that represents the border of the object |
### Example
```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.pydrawing import Color
# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
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
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 25, 10)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
chart.show_data_table = True
# Getting Chart Table
chartTable = chart.chart_data_table
# Setting Chart Table Font Color
chartTable.font.color = Color.red
# Setting Legend Key VisibilityOptions
chartTable.show_legend_key = False
# Saving the Excel file
workbook.save("book1.xls")
```
### See Also
* module [`aspose.cells.charts`](..)
