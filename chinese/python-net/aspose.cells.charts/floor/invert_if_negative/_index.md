---
title: invert_if_negative 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 80
url: /zh/python-net/aspose.cells.charts/floor/invert_if_negative/
is_root: false
---
## invert_if_negative 属性

如果该属性为真且图表点的值为负数，
前景色和背景色将交换。

### 例子

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
worksheet.cells.get("A2").put_value(-100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
chart.n_series.add("A1:A3", True)
chart.n_series[0].area.invert_if_negative = True
# Setting the foreground color of the 1st NSeries area
chart.n_series[0].area.foreground_color = Color.red
# Setting the background color of the 1st NSeries area.
# The displayed area color of second chart point will be the background color.
chart.n_series[0].area.background_color = Color.yellow
# Saving the Excel file
workbook.save("book1.xls")

```
### 定义：
```python
@property
def invert_if_negative(self):
    ...
@invert_if_negative.setter
def invert_if_negative(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells.charts](../../)
* 类 [Floor](/cells/zh/python-net/aspose.cells.charts/floor)
