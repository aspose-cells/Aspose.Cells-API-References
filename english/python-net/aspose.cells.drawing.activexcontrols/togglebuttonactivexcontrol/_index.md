---
title: ToggleButtonActiveXControl class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 130
url: /python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/
is_root: false
---

## ToggleButtonActiveXControl class

Represents a ToggleButton ActiveX control.



**Inheritance:** [ToggleButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



The ToggleButtonActiveXControl type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [workbook](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/workbook) | Gets the [ActiveXControlBase.workbook](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook) object. |
| [type](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/type) | Gets the type of the ActiveX control. |
| [width](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/width) | Gets and sets the width of the control in unit of points. |
| [height](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/height) | Gets and sets the height of the control in unit of points. |
| [mouse_icon](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_icon) | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [mouse_pointer](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_pointer) | Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [fore_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/fore_ole_color) | Gets and sets the ole color of the foreground. |
| [back_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/back_ole_color) | Gets and sets the ole color of the background. |
| [is_visible](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_visible) | Indicates whether this control is visible. |
| [shadow](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/shadow) | Indicates whether to show a shadow. |
| [linked_cell](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/linked_cell) | Gets and sets the linked cell. |
| [list_fill_range](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/list_fill_range) | Gets and sets the list fill range. |
| [data](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/data) | Gets and sets the binary data of the control. |
| [is_enabled](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_enabled) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [is_locked](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_locked) | Indicates whether data in the control is locked for editing. |
| [is_transparent](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_transparent) | Indicates whether the control is transparent. |
| [is_auto_size](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_auto_size) | Indicates whether the control will automatically resize to display its entire contents. |
| [ime_mode](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/ime_mode) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [font](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/font) | Represents the font of the control. |
| [text_align](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/text_align) | Represents how to align the text used by the control. |
| [caption](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/caption) | Gets and set the descriptive text that appears on a control. |
| [picture_position](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture_position) | Gets and set the location of the control's picture relative to its caption. |
| [special_effect](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/special_effect) | Gets and sets the special effect of the control. |
| [picture](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture) | Gets and sets the data of the picture. |
| [accelerator](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/accelerator) | Gets and sets the accelerator key for the control. |
| [value](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value) | Indicates if the control is checked or not. |
| [is_triple_state](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_triple_state) | Indicates how the specified control will display Null values. |



### Example 


```python
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType
import aspose.pycore

# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.TOGGLE_BUTTON, 1, 0, 1, 0, 100, 50)
activeXControl = aspose.pycore.cast(Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")

```
### See Also

* module [aspose.cells.drawing.activexcontrols](../)
* class [ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
