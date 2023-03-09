---
title: minor_unit_scale 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 360
url: /zh/python-net/aspose.cells.charts/axis/minor_unit_scale/
is_root: false
---
## minor_unit_scale 属性

表示类别轴的主要单位刻度。

### 例子

```python
from aspose.cells.charts import CategoryType, TimeUnit

chart.category_axis.category_type = CategoryType.TIME_SCALE
chart.category_axis.minor_unit_scale = TimeUnit.MONTHS
chart.category_axis.minor_unit = 2

```
### 定义：
```python
@property
def minor_unit_scale(self):
    ...
@minor_unit_scale.setter
def minor_unit_scale(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells.charts](../../)
* 类 [Axis](/cells/zh/python-net/aspose.cells.charts/axis)
* 类 [TimeUnit](/cells/zh/python-net/aspose.cells.charts/timeunit)
