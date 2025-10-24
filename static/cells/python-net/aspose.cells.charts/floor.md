##Floor class
## Floor class
Encapsulates the object that represents the floor of a 3-D chart.
**Inheritance:** [`Floor`](/cells/python-net/aspose.cells.charts/floor) →
[`Area`](/cells/python-net/aspose.cells.drawing/area)
The Floor type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [background_color](/cells/python-net/aspose.cells.charts/floor/background_color) | Gets or sets the background Color of the [`Area`](/cells/python-net/aspose.cells.drawing/area). |
| [foreground_color](/cells/python-net/aspose.cells.charts/floor/foreground_color) | Gets or sets the foreground Color. |
| [formatting](/cells/python-net/aspose.cells.charts/floor/formatting) | Represents the formatting of the area. |
| [invert_if_negative](/cells/python-net/aspose.cells.charts/floor/invert_if_negative) | If the property is true and the value of chart point is a negative number,
| [fill_format](/cells/python-net/aspose.cells.charts/floor/fill_format) | Represents a [`Area.fill_format`](/cells/python-net/aspose.cells.drawing/area#fill_format) object that contains fill formatting properties for the specified chart or shape. |
| [transparency](/cells/python-net/aspose.cells.charts/floor/transparency) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [border](/cells/python-net/aspose.cells.charts/floor/border) | Gets or sets the border [`Line`](/cells/python-net/aspose.cells.drawing/line). |
### Example
```python
from aspose.cells import License, Workbook
from aspose.cells.charts import ChartType
from aspose.cells.drawing import GradientPresetType, GradientStyleType
from aspose.pydrawing import Color
# Instantiate the License class
license = License()
# Pass only the name of the license file embedded in the assembly
license.set_license("Aspose.Cells.lic")
# Instantiate the workbook object
workbook = Workbook()
# Get cells collection
cells = workbook.worksheets[0].cells
# Put values in cells
cells.get("A1").put_value(1)
cells.get("A2").put_value(2)
cells.get("A3").put_value(3)
# get charts colletion
charts = workbook.worksheets[0].charts
# add a new chart
index = charts.add(ChartType.COLUMN_3D_STACKED, 5, 0, 15, 5)
# get the newly added chart
chart = charts[index]
# set charts nseries
chart.n_series.add("A1:A3", True)
# Show data labels
chart.n_series[0].data_labels.show_value = True
# Get chart's floor
floor = chart.floor
# set floor's border as red
floor.border.color = Color.red
# set fill format
floor.fill_format.set_preset_color_gradient(GradientPresetType.CALM_WATER, GradientStyleType.DIAGONAL_DOWN, 2)
# save the file
workbook.save(r"dest.xls")
```
### See Also
* module [`aspose.cells.charts`](..)
* class [`Area`](/cells/python-net/aspose.cells.drawing/area)
* class [`Floor`](/cells/python-net/aspose.cells.charts/floor)
* class [`Line`](/cells/python-net/aspose.cells.drawing/line)
