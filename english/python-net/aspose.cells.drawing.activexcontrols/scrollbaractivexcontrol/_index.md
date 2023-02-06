---
title: ScrollBarActiveXControl class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 100
url: /python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/
is_root: false
---

## ScrollBarActiveXControl class

Represents the ScrollBar control.



**Inheritance:** [ScrollBarActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol) → 
[SpinButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



The ScrollBarActiveXControl type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [workbook](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/workbook) | Gets the [ActiveXControlBase.workbook](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook) object. |
| [type](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/type) | Gets the type of the ActiveX control. |
| [width](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/width) | Gets and sets the width of the control in unit of points. |
| [height](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/height) | Gets and sets the height of the control in unit of points. |
| [mouse_icon](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/mouse_icon) | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [mouse_pointer](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/mouse_pointer) | Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [fore_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/fore_ole_color) | Gets and sets the ole color of the foreground. |
| [back_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/back_ole_color) | Gets and sets the ole color of the background. |
| [is_visible](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_visible) | Indicates whether this control is visible. |
| [shadow](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/shadow) | Indicates whether to show a shadow. |
| [linked_cell](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/linked_cell) | Gets and sets the linked cell. |
| [list_fill_range](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/list_fill_range) | Gets and sets the list fill range. |
| [data](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/data) | Gets and sets the binary data of the control. |
| [is_enabled](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_enabled) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [is_locked](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_locked) | Indicates whether data in the control is locked for editing. |
| [is_transparent](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_transparent) | Indicates whether the control is transparent. |
| [is_auto_size](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_auto_size) | Indicates whether the control will automatically resize to display its entire contents. |
| [ime_mode](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/ime_mode) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [font](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/font) | Represents the font of the control. |
| [text_align](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/text_align) | Represents how to align the text used by the control. |
| [min](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/min) | Gets and sets the minimum acceptable value. |
| [max](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/max) | Gets and sets the maximum acceptable value. |
| [position](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/position) | Gets and sets the value. |
| [small_change](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/small_change) | Gets and sets the amount by which the Position property changes |
| [orientation](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/orientation) | Gets and sets whether the SpinButton or ScrollBar is oriented vertically or horizontally. |
| [large_change](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/large_change) | Gets and sets the amount by which the Position property changes |



### Example 


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

### See Also
* module [aspose.cells.drawing.activexcontrols](..)
* class [ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* class [ActiveXControlBase](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* class [ScrollBarActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol)
* class [SpinButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)
