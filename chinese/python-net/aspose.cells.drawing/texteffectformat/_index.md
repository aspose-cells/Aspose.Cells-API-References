---
title: TextEffectFormat类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 700
url: /zh/python-net/aspose.cells.drawing/texteffectformat/
is_root: false
---
## TextEffectFormat类
包含适用于艺术字对象的属性和方法。



TextEffectFormat 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [text](/cells/zh/python-net/aspose.cells.drawing/texteffectformat/text) |艺术字中的文本。|
| [font_name](/cells/zh/python-net/aspose.cells.drawing/texteffectformat/font_name) |艺术字中使用的字体名称。|
| [font_bold](/cells/zh/python-net/aspose.cells.drawing/texteffectformat/font_bold) |指示字体是否为粗体。|
| [font_italic](/cells/zh/python-net/aspose.cells.drawing/texteffectformat/font_italic) |指示字体是否为斜体。|
| [rotated_chars](/cells/zh/python-net/aspose.cells.drawing/texteffectformat/rotated_chars) |如果为 true，则指定艺术字中的字符相对于艺术字的边界形状旋转 90 度。|
| [font_size](/cells/zh/python-net/aspose.cells.drawing/texteffectformat/font_size) |艺术字中使用的字体大小（以磅为单位）。|
| [preset_shape](/cells/zh/python-net/aspose.cells.drawing/texteffectformat/preset_shape) |获取和设置预设形状类型。|


### 方法
|方法|描述|
| :- | :- |
| [set_text_effect(effect)](/cells/zh/python-net/aspose.cells.drawing/texteffectformat/set_text_effect/#MsoPresetTextEffect) |设置预设文本效果。|



### 例子

```python
from aspose.cells import Workbook
from aspose.cells.drawing import MsoPresetTextEffect

# Instantiating a Workbook object
workbook = Workbook()
shapes = workbook.worksheets[0].shapes
shapes.add_text_effect(MsoPresetTextEffect.TEXT_EFFECT1, "Aspose", "Arial", 30, False, False, 0, 0, 0, 0, 100, 200)
textEffectFormat = shapes[0].text_effect
textEffectFormat.set_text_effect(MsoPresetTextEffect.TEXT_EFFECT10)
workbook.save("Book1.xls")

```

### 也可以看看
* 模块 [aspose.cells.drawing](..)
