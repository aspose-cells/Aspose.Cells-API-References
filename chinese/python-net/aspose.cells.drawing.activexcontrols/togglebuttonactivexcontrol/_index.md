---
title: ToggleButtonActiveXControl类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 130
url: /zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/
is_root: false
---
## ToggleButtonActiveXControl类
表示 ToggleButton ActiveX 控件。



**继承：** [ToggleButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



ToggleButtonActiveXControl 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [workbook](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/workbook) |获取 [ActiveXControlBase.workbook](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook) 对象。|
| [type](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/type) |获取 ActiveX 控件的类型。|
| [width](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/width) |以点为单位获取和设置控件的宽度。|
| [height](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/height) |以点为单位获取和设置控件的高度。|
| [mouse_icon](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_icon) |获取并设置一个自定义图标以显示为控件的鼠标指针。|
| [mouse_pointer](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_pointer) |获取和设置显示为控件鼠标指针的图标类型。|
| [fore_ole_color](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/fore_ole_color) |获取和设置前景的 ole 颜色。|
| [back_ole_color](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/back_ole_color) |获取和设置背景的 ole 颜色。|
| [is_visible](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_visible) |指示此控件是否可见。|
| [shadow](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/shadow) |指示是否显示阴影。|
| [linked_cell](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/linked_cell) |获取和设置链接的单元格。|
| [list_fill_range](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/list_fill_range) |获取和设置列表填充范围。|
| [data](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/data) |获取和设置控件的二进制数据。|
| [is_enabled](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_enabled) |指示控件是否可以接收焦点并响应用户生成的事件。|
| [is_locked](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_locked) |指示控件中的数据是否已锁定以供编辑。|
| [is_transparent](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_transparent) |指示控件是否透明。|
| [is_auto_size](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_auto_size) |指示控件是否会自动调整大小以显示其全部内容。|
| [ime_mode](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/ime_mode) |获取和设置控件接收焦点时输入法编辑器的默认运行时模式。|
| [font](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/font) |表示控件的字体。|
| [text_align](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/text_align) |表示如何对齐控件使用的文本。|
| [caption](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/caption) |获取和设置出现在控件上的描述性文本。|
| [picture_position](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture_position) |获取和设置控件图片相对于其标题的位置。|
| [special_effect](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/special_effect) |获取和设置控件的特殊效果。|
| [picture](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture) |获取和设置图片的数据。|
| [accelerator](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/accelerator) |获取和设置控件的快捷键。|
| [value](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value) |指示控件是否已选中。|
| [is_triple_state](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_triple_state) |指示指定的控件将如何显示 Null 值。|



### 例子

```python
from aspose import pycore
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType, ToggleButtonActiveXControl

# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.TOGGLE_BUTTON, 1, 0, 1, 0, 100, 50)
activeXControl = pycore.cast(ToggleButtonActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")

```

### 也可以看看
* 模块 [aspose.cells.drawing.activexcontrols](..)
* 类 [ActiveXControl](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* 类 [ActiveXControlBase](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* 类 [ToggleButtonActiveXControl](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol)
