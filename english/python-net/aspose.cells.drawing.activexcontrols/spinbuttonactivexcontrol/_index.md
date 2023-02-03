---
title: SpinButtonActiveXControl class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 110
url: /python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/
is_root: false
---

## SpinButtonActiveXControl class

Represents the SpinButton control.



**Inheritance:** [SpinButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



The SpinButtonActiveXControl type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [workbook](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/workbook) | Gets the [ActiveXControlBase.workbook](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook) object. |
| [type](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type) | Gets the type of the ActiveX control. |
| [width](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/width) | Gets and sets the width of the control in unit of points. |
| [height](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/height) | Gets and sets the height of the control in unit of points. |
| [mouse_icon](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_icon) | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [mouse_pointer](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_pointer) | Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [fore_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/fore_ole_color) | Gets and sets the ole color of the foreground. |
| [back_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/back_ole_color) | Gets and sets the ole color of the background. |
| [is_visible](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_visible) | Indicates whether this control is visible. |
| [shadow](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/shadow) | Indicates whether to show a shadow. |
| [linked_cell](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/linked_cell) | Gets and sets the linked cell. |
| [list_fill_range](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/list_fill_range) | Gets and sets the list fill range. |
| [data](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/data) | Gets and sets the binary data of the control. |
| [is_enabled](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_enabled) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [is_locked](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_locked) | Indicates whether data in the control is locked for editing. |
| [is_transparent](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_transparent) | Indicates whether the control is transparent. |
| [is_auto_size](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_auto_size) | Indicates whether the control will automatically resize to display its entire contents. |
| [ime_mode](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/ime_mode) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [font](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/font) | Represents the font of the control. |
| [text_align](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/text_align) | Represents how to align the text used by the control. |
| [min](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min) | Gets and sets the minimum acceptable value. |
| [max](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max) | Gets and sets the maximum acceptable value. |
| [position](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position) | Gets and sets the value. |
| [small_change](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/small_change) | Gets and sets the amount by which the Position property changes |
| [orientation](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation) | Gets and sets whether the SpinButton or ScrollBar is oriented vertically or horizontally. |



### Example 


```python
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType
import aspose.pycore

# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.SPIN_BUTTON, 1, 0, 1, 0, 100, 50)
activeXControl = aspose.pycore.cast(Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")

```
### See Also

* module [aspose.cells.drawing.activexcontrols](../)
* class [ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
