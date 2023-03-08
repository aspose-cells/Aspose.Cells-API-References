---
title: set_two_color_gradient方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/
is_root: false
---
##  set_two_color_gradient(color1, color2, style, variant) {#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int}
将指定的填充设置为双色渐变。
仅适用于 Excel 2007。



```python
def set_two_color_gradient(self, color1, color2, style, variant):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color |一种渐变色。|
| color2 | aspose.pydrawing.Color |两种渐变色。|
| style | [GradientStyleType](/cells/zh/python-net/aspose.cells.drawing/gradientstyletype) |渐变阴影样式。|
| variant | int |渐变变体。可以是 1 到 4 之间的值，对应于“填充效果”对话框中“渐变”选项卡上的四个变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。|


##  set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant) {#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int}
将指定的填充设置为双色渐变。
仅适用于 Excel 2007。



```python
def set_two_color_gradient(self, color1, transparency1, color2, transparency2, style, variant):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| color1 | aspose.pydrawing.Color |一种渐变色。|
| transparency1 | float | color1 的透明度，值为从 0.0（不透明）到 1.0（透明）的值。|
| color2 | aspose.pydrawing.Color |两种渐变色。|
| transparency2 | float | color2 的透明度，值为从 0.0（不透明）到 1.0（透明）的值。|
| style | [GradientStyleType](/cells/zh/python-net/aspose.cells.drawing/gradientstyletype) |渐变阴影样式。|
| variant | int |渐变变体。可以是 1 到 4 之间的值，对应于“填充效果”对话框中“渐变”选项卡上的四个变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。|



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [FillFormat](/cells/zh/python-net/aspose.cells.drawing/fillformat)
