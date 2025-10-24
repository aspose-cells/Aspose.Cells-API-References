##RadioButtonActiveXControl class
## RadioButtonActiveXControl class
Represents a RadioButton ActiveX control.
**Inheritance:** [`RadioButtonActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol) →
[`ToggleButtonActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol)
The RadioButtonActiveXControl type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [workbook](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/workbook) |  |
| [type](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/type) | Gets the type of the ActiveX control. |
| [width](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/width) |  |
| [height](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/height) |  |
| [mouse_icon](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/mouse_icon) |  |
| [mouse_pointer](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/mouse_pointer) |  |
| [fore_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/fore_ole_color) |  |
| [back_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/back_ole_color) |  |
| [is_visible](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/is_visible) |  |
| [shadow](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/shadow) |  |
| [linked_cell](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/linked_cell) |  |
| [list_fill_range](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/list_fill_range) |  |
| [data](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/data) |  |
| [is_enabled](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/is_enabled) |  |
| [is_locked](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/is_locked) |  |
| [is_transparent](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/is_transparent) |  |
| [is_auto_size](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/is_auto_size) |  |
| [ime_mode](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/ime_mode) |  |
| [font](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/font) |  |
| [text_align](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/text_align) |  |
| [caption](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/caption) | Gets and set the descriptive text that appears on a control. |
| [picture_position](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/picture_position) | Gets and set the location of the control's picture relative to its caption. |
| [special_effect](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/special_effect) | Gets and sets the special effect of the control. |
| [picture](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/picture) | Gets and sets the data of the picture. |
| [accelerator](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/accelerator) | Gets and sets the accelerator key for the control. |
| [value](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/value) | Indicates if the control is checked or not. |
| [is_triple_state](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/is_triple_state) | Indicates how the specified control will display Null values. |
| [group_name](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/group_name) | Gets and sets the group's name. |
| [alignment](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/alignment) | Gets and set the position of the Caption relative to the control. |
| [is_word_wrapped](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/is_word_wrapped) | Indicates whether the contents of the control automatically wrap at the end of a line. |
### Example
```python
from aspose import pycore
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType, RadioButtonActiveXControl
# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.RADIO_BUTTON, 1, 0, 1, 0, 100, 50)
activeXControl = pycore.cast(RadioButtonActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")
```
### See Also
* module [`aspose.cells.drawing.activexcontrols`](..)
* class [`RadioButtonActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol)
* class [`ToggleButtonActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol)
