---
title: calculate_data方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells.pivot/pivottable/calculate_data/
is_root: false
---
##  calculate_data() {#}
将数据透视表的数据计算到单元格。



```python
def calculate_data(self):
    ...
```


### 评论

Cell.如果不调用该方法，枢轴范围内的值无法返回正确的结果。
此方法使用内部数据透视缓存而不是原始数据源计算数据。
所以如果数据源改变了，请先调用RefreshData()方法。


### 也可以看看
* 模块 [aspose.cells.pivot](../../)
* 类 [PivotTable](/cells/zh/python-net/aspose.cells.pivot/pivottable)
