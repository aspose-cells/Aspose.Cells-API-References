---
title: is_chart_data_changed方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 70
url: /zh/python-net/aspose.cells.charts/chart/is_chart_data_changed/
is_root: false
---
##  is_chart_data_changed() {#}
检测图表的数据源是否已更改。


### 返回

如果图表已更改，则返回 true 否则返回 false


```python
def is_chart_data_changed(self):
    ...
```


### 评论

该方法在将图表呈现为图像格式之前检测图表数据源的变化。
在第一次调用 Chart.toImage 时，图表源数据（例如 XValuesParseData、ValuesParseData）将被记录下来。
在再次调用 Chart.toImage 方法之前，调用 IsChartDataChanged 方法检查 Chart 是否需要重新渲染。


### 也可以看看
* 模块 [aspose.cells.charts](../../)
* 类 [Chart](/cells/zh/python-net/aspose.cells.charts/chart)
