---
title: ScrollBarActiveXControl类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 100
url: /zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/
is_root: false
---
## ScrollBarActiveXControl类
表示滚动条控件。



**继承：** [ScrollBarActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol) → 
[SpinButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



ScrollBarActiveXControl 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [workbook](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/workbook) |获取 [ActiveXControlBase.workbook](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook) 对象。|
| [type](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/type) |获取 ActiveX 控件的类型。|
| [width](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/width) |以点为单位获取和设置控件的宽度。|
| [height](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/height) |以点为单位获取和设置控件的高度。|
| [mouse_icon](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/mouse_icon) |获取并设置一个自定义图标以显示为控件的鼠标指针。|
| [mouse_pointer](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/mouse_pointer) |获取和设置显示为控件鼠标指针的图标类型。|
| [fore_ole_color](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/fore_ole_color) |获取和设置前景的 ole 颜色。|
| [back_ole_color](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/back_ole_color) |获取和设置背景的 ole 颜色。|
| [is_visible](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_visible) |指示此控件是否可见。|
| [shadow](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/shadow) |指示是否显示阴影。|
| [linked_cell](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/linked_cell) |获取和设置链接的单元格。|
| [list_fill_range](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/list_fill_range) |获取和设置列表填充范围。|
| [data](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/data) |获取和设置控件的二进制数据。|
| [is_enabled](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_enabled) |指示控件是否可以接收焦点并响应用户生成的事件。|
| [is_locked](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_locked) |指示控件中的数据是否已锁定以供编辑。|
| [is_transparent](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_transparent) |指示控件是否透明。|
| [is_auto_size](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_auto_size) |指示控件是否会自动调整大小以显示其全部内容。|
| [ime_mode](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/ime_mode) |获取和设置控件接收焦点时输入法编辑器的默认运行时模式。|
| [font](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/font) |表示控件的字体。|
| [text_align](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/text_align) |表示如何对齐控件使用的文本。|
| [min](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/min) |获取并设置最小可接受值。|
| [max](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/max) |获取和设置最大可接受值。|
| [position](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/position) |获取和设置值。|
| [small_change](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/small_change) |获取和设置 Position 属性变化的量|
| [orientation](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/orientation) |获取和设置 SpinButton 或 ScrollBar 是垂直方向还是水平方向。|
| [large_change](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/large_change) |获取和设置 Position 属性变化的量|



### 例子

```python
from aspose import pycore
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType, ScrollBarActiveXControl

# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.SCROLL_BAR, 1, 0, 1, 0, 100, 50)
activeXControl = pycore.cast(ScrollBarActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")

```

### 也可以看看
* 模块 [aspose.cells.drawing.activexcontrols](..)
* 类 [ActiveXControl](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* 类 [ActiveXControlBase](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* 类 [ScrollBarActiveXControl](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol)
* 类 [SpinButtonActiveXControl](/cells/zh/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)
