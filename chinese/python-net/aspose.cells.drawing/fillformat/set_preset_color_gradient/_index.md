---
title: set_preset_color_gradient方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells.drawing/fillformat/set_preset_color_gradient/
is_root: false
---
##  set_preset_color_gradient(preset_color, style, variant) {#GradientPresetType-GradientStyleType-int}
将指定的填充设置为预设颜色渐变。
仅适用于 Excel 2007。



```python
def set_preset_color_gradient(self, preset_color, style, variant):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| preset_color | [GradientPresetType](/cells/zh/python-net/aspose.cells.drawing/gradientpresettype) |预设颜色类型|
| style | [GradientStyleType](/cells/zh/python-net/aspose.cells.drawing/gradientstyletype) |渐变阴影样式。|
| variant | int |渐变变体。可以是 1 到 4 之间的值，对应于“填充效果”对话框中“渐变”选项卡上的四个变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。|



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [FillFormat](/cells/zh/python-net/aspose.cells.drawing/fillformat)
