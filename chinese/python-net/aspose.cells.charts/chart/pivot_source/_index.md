---
title: pivot_source 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 400
url: /zh/python-net/aspose.cells.charts/chart/pivot_source/
is_root: false
---
## pivot_source 属性

源是数据透视表的数据。
如果 PivotSource 不为空，则图表为 PivotChart。

### 评论

如文件“Book1.xls”中工作表“Sheet1”中的数据透视表“PivotTable1”。
如果图表和数据透视表不在同一个工作簿中，数据透视表源可以是“[Book1.xls]Sheet1!PivotTable1”。
如果你设置了这个属性，之前的数据源设置将会丢失。
### 定义：
```python
@property
def pivot_source(self):
    ...
@pivot_source.setter
def pivot_source(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells.charts](../../)
* 类 [Chart](/cells/zh/python-net/aspose.cells.charts/chart)
