---
title: x 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 270
url: /zh/python-net/aspose.cells.charts/plotarea/x/
is_root: false
---
## x 属性

获取或获取绘图区域边界框左上角的x坐标，以图表区域的1/4000为单位。

### 评论

绘图区域边界框包括绘图区域、刻度线（刻度标签）和刻度线周围的小边框。
如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。


这**X** , **Y** , **宽度**和**高度**的**绘图区**代表地块面积
一个边界框，包括绘图区域、刻度线（刻度标签）和刻度线周围的小边框。
如果你想获得绘图区域的实际大小，你应该调用**内X** , **内 Y** , **内宽**和
**内部高度**特性。


对于 excel 2007 或更高版本，默认值为零。
### 定义：
```python
@property
def x(self):
    ...
@x.setter
def x(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells.charts](../../)
* 类 [PlotArea](/cells/zh/python-net/aspose.cells.charts/plotarea)
