---
title: ChartPointCollection类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 100
url: /zh/python-net/aspose.cells.charts/chartpointcollection/
is_root: false
---
## ChartPointCollection类
表示包含一个系列中所有点的集合。



ChartPointCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [count](/cells/zh/python-net/aspose.cells.charts/chartpointcollection/count) |获取图表点的计数。|



获取系列中指定索引处的 [ChartPoint](/cells/zh/python-net/aspose.cells.charts/chartpoint) 元素。
### 索引器
|名称|描述|
| :- | :- |
| [index] |系列中图表点的索引。|


### 方法
|方法|描述|
| :- | :- |
| [get_enumerator()](/cells/zh/python-net/aspose.cells.charts/chartpointcollection/get_enumerator/#) |返回整个 [ChartPointCollection](/cells/zh/python-net/aspose.cells.charts/chartpointcollection) 的枚举器。|
| [clear()](/cells/zh/python-net/aspose.cells.charts/chartpointcollection/clear/#) |删除图表点的所有设置。|
| [remove_at(index)](/cells/zh/python-net/aspose.cells.charts/chartpointcollection/remove_at/#int) |删除系列索引处的点..|



### 例子

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
chartIndex = worksheet.charts.add(ChartType.PIE_EXPLODED, 5, 0, 25, 10)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Show Data Labels
chart.n_series[0].data_labels.show_value = True
points = chart.n_series[0].points
for i in range(points.count):
    # Get Data Point
    point = points[i]
    # Set Pir Explosion
    point.explosion = 15
    # Set Border Color
    point.border.color = Color.red
# Saving the Excel file
workbook.save("book1.xls")

```

### 也可以看看
* 模块 [aspose.cells.charts](..)
* 类 [ChartPoint](/cells/zh/python-net/aspose.cells.charts/chartpoint)
* 类 [ChartPointCollection](/cells/zh/python-net/aspose.cells.charts/chartpointcollection)
