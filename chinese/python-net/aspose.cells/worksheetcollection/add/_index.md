---
title: add方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/worksheetcollection/add/
is_root: false
---
##  add() {#}
将工作表添加到集合中。


### 返回

[Worksheet](/cells/zh/python-net/aspose.cells/worksheet) 对象索引。


```python
def add(self):
    ...
```




##  add(type) {#SheetType}
将工作表添加到集合中。


### 返回

[Worksheet](/cells/zh/python-net/aspose.cells/worksheet) 对象索引。


```python
def add(self, type):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [SheetType](/cells/zh/python-net/aspose.cells/sheettype) |工作表类型。|

### 例子

```python
from aspose.cells import SheetType, Workbook
from aspose.cells.charts import ChartType

workbook = Workbook()
workbook.worksheets.add(SheetType.CHART)
cells = workbook.worksheets[0].cells
cells.get("c2").put_value(5000)
cells.get("c3").put_value(3000)
cells.get("c4").put_value(4000)
cells.get("c5").put_value(5000)
cells.get("c6").put_value(6000)
charts = workbook.worksheets[1].charts
chartIndex = charts.add(ChartType.COLUMN, 10, 10, 20, 20)
chart = charts[chartIndex]
chart.n_series.add("Sheet1!C2:C6", True)

```


##  add(sheet_name) {#str}
将工作表添加到集合中。


### 返回

[Worksheet](/cells/zh/python-net/aspose.cells/worksheet) 对象。


```python
def add(self, sheet_name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| sheet_name | str |工作表名称|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Worksheet](/cells/zh/python-net/aspose.cells/worksheet)
* 类 [WorksheetCollection](/cells/zh/python-net/aspose.cells/worksheetcollection)
