##ToggleButtonActiveXControl class
## ToggleButtonActiveXControl class
Represents a ToggleButton ActiveX control.
**Inheritance:** [`ToggleButtonActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol)
The ToggleButtonActiveXControl type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [workbook](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/workbook) |  |
| [type](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/type) | Gets the type of the ActiveX control. |
| [width](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/width) |  |
| [height](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/height) |  |
| [mouse_icon](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_icon) |  |
| [mouse_pointer](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/mouse_pointer) |  |
| [fore_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/fore_ole_color) |  |
| [back_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/back_ole_color) |  |
| [is_visible](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_visible) |  |
| [shadow](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/shadow) |  |
| [linked_cell](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/linked_cell) |  |
| [list_fill_range](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/list_fill_range) |  |
| [data](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/data) |  |
| [is_enabled](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_enabled) |  |
| [is_locked](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_locked) |  |
| [is_transparent](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_transparent) |  |
| [is_auto_size](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_auto_size) |  |
| [ime_mode](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/ime_mode) |  |
| [font](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/font) |  |
| [text_align](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/text_align) |  |
| [caption](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/caption) | Gets and set the descriptive text that appears on a control. |
| [picture_position](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture_position) | Gets and set the location of the control's picture relative to its caption. |
| [special_effect](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/special_effect) | Gets and sets the special effect of the control. |
| [picture](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture) | Gets and sets the data of the picture. |
| [accelerator](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/accelerator) | Gets and sets the accelerator key for the control. |
| [value](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value) | Indicates if the control is checked or not. |
| [is_triple_state](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/is_triple_state) | Indicates how the specified control will display Null values. |
### Example
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
### See Also
* module [`aspose.cells.drawing.activexcontrols`](..)
* class [`ToggleButtonActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol)
