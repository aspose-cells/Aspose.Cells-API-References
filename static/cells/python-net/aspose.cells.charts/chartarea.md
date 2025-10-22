##ChartArea class
## ChartArea class
Encapsulates the object that represents the chart area in the worksheet.
**Inheritance:** [`ChartArea`](/cells/python-net/aspose.cells.charts/chartarea) →
[`ChartFrame`](/cells/python-net/aspose.cells.charts/chartframe)
The ChartArea type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [is_inner_mode](/cells/python-net/aspose.cells.charts/chartarea/is_inner_mode) | Indicates whether the size of the plot area size includes the tick marks, and the axis labels.
| [border](/cells/python-net/aspose.cells.charts/chartarea/border) | Gets the [`Line`](/cells/python-net/aspose.cells.drawing/line). |
| [area](/cells/python-net/aspose.cells.charts/chartarea/area) | Gets the [`ChartFrame.area`](/cells/python-net/aspose.cells.charts/chartframe#area). |
| [text_font](/cells/python-net/aspose.cells.charts/chartarea/text_font) | Gets a [`ChartFrame.font`](/cells/python-net/aspose.cells.charts/chartframe#font) object of the specified ChartFrame object. |
| [text_options](/cells/python-net/aspose.cells.charts/chartarea/text_options) | Gets and sets the options of the text. |
| [font](/cells/python-net/aspose.cells.charts/chartarea/font) | Gets a [`ChartArea.font`](/cells/python-net/aspose.cells.charts/chartarea#font) object of the specified chartarea object. |
| [auto_scale_font](/cells/python-net/aspose.cells.charts/chartarea/auto_scale_font) | True if the text in the object changes font size when the object size changes. The default value is True. |
| [background_mode](/cells/python-net/aspose.cells.charts/chartarea/background_mode) | Gets and sets the display mode of the background |
| [background](/cells/python-net/aspose.cells.charts/chartarea/background) | Gets and sets the display mode of the background |
| [is_automatic_size](/cells/python-net/aspose.cells.charts/chartarea/is_automatic_size) | Indicates whether the chart frame is automatic sized. |
| [x](/cells/python-net/aspose.cells.charts/chartarea/x) | Gets or gets the horizontal offset from its upper left corner column, in units of 1/4000 of the chart area. |
| [y](/cells/python-net/aspose.cells.charts/chartarea/y) | Gets or gets the vertical offset from its upper left corner row, in units of 1/4000 of the chart area. |
| [height](/cells/python-net/aspose.cells.charts/chartarea/height) | Gets or sets the vertical offset from its lower right corner row, in units of 1/4000 of the chart area. |
| [width](/cells/python-net/aspose.cells.charts/chartarea/width) | Gets or sets the horizontal offset from its lower right corner column, in units of 1/4000 of the chart area. |
| [shadow](/cells/python-net/aspose.cells.charts/chartarea/shadow) | True if the frame has a shadow. |
| [shape_properties](/cells/python-net/aspose.cells.charts/chartarea/shape_properties) | Gets the [`ChartFrame.shape_properties`](/cells/python-net/aspose.cells.charts/chartframe#shape_properties) object. |
| [is_default_pos_be_set](/cells/python-net/aspose.cells.charts/chartarea/is_default_pos_be_set) | Indicates whether default position(DefaultX, DefaultY, DefaultWidth and DefaultHeight) are set. |
| [default_x](/cells/python-net/aspose.cells.charts/chartarea/default_x) | Represents x of default position in units of 1/4000 of the chart area. |
| [default_y](/cells/python-net/aspose.cells.charts/chartarea/default_y) | Represents y of default position in units of 1/4000 of the chart area. |
| [default_width](/cells/python-net/aspose.cells.charts/chartarea/default_width) | Represents width of default position in units of 1/4000 of the chart area. |
| [default_height](/cells/python-net/aspose.cells.charts/chartarea/default_height) | Represents height of default position in units of 1/4000 of the chart area. |
| [default_x_ratio_to_chart](/cells/python-net/aspose.cells.charts/chartarea/default_x_ratio_to_chart) | Represents x of default position in units of Fraction of the chart area. |
| [default_y_ratio_to_chart](/cells/python-net/aspose.cells.charts/chartarea/default_y_ratio_to_chart) | Represents y of default position in units of Fraction of the chart area. |
| [default_width_ratio_to_chart](/cells/python-net/aspose.cells.charts/chartarea/default_width_ratio_to_chart) | Represents width of default position in units of Fraction of the chart area. |
| [default_height_ratio_to_chart](/cells/python-net/aspose.cells.charts/chartarea/default_height_ratio_to_chart) | Represents height of default position in units of Fraction of the chart area. |
| [x_ratio_to_chart](/cells/python-net/aspose.cells.charts/chartarea/x_ratio_to_chart) | Gets or gets the horizontal offset from its upper left corner column, in units of ratio of the chart area. |
| [y_ratio_to_chart](/cells/python-net/aspose.cells.charts/chartarea/y_ratio_to_chart) | Gets or gets the vertical offset from its upper left corner row, in units of ratio of the chart area. |
| [width_ratio_to_chart](/cells/python-net/aspose.cells.charts/chartarea/width_ratio_to_chart) | Gets or sets the horizontal offset from its lower right corner column, in units of ratio of the chart area. |
| [height_ratio_to_chart](/cells/python-net/aspose.cells.charts/chartarea/height_ratio_to_chart) | Gets or sets the vertical offset from its lower right corner row, in units of ratio of the chart area. |
| [x_pixel](/cells/python-net/aspose.cells.charts/chartarea/x_pixel) | Gets or sets the x coordinate of the upper left corner in units of Pixel. |
| [y_pixel](/cells/python-net/aspose.cells.charts/chartarea/y_pixel) | Gets or sets the y coordinate of the upper left corner in units of Pixel. |
| [width_pixel](/cells/python-net/aspose.cells.charts/chartarea/width_pixel) | Gets or sets the width of frame in units of Pixel. |
| [height_pixel](/cells/python-net/aspose.cells.charts/chartarea/height_pixel) | Gets or sets the height of frame in units of Pixel. |
### Methods
| Method | Description |
| :- | :- |
| [`set_position_auto(self)`](/cells/python-net/aspose.cells.charts/chartarea/set_position_auto/#) | Set position of the frame to automatic |
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
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Getting Chart Area
chartArea = chart.chart_area
# Setting the foreground color of the chart area
chartArea.area.foreground_color = Color.yellow
# Setting Chart Area Shadow
chartArea.shadow = True
# Saving the Excel file
workbook.save("book1.xls")
```
### See Also
* module [`aspose.cells.charts`](..)
* class [`ChartArea`](/cells/python-net/aspose.cells.charts/chartarea)
* class [`ChartFrame`](/cells/python-net/aspose.cells.charts/chartframe)
* class [`Line`](/cells/python-net/aspose.cells.drawing/line)
