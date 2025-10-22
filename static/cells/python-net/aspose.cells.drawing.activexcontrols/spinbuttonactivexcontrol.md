##SpinButtonActiveXControl class
## SpinButtonActiveXControl class
Represents the SpinButton control.
**Inheritance:** [`SpinButtonActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)
The SpinButtonActiveXControl type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [workbook](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/workbook) |  |
| [type](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type) | Gets the type of the ActiveX control. |
| [width](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/width) |  |
| [height](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/height) |  |
| [mouse_icon](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_icon) |  |
| [mouse_pointer](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/mouse_pointer) |  |
| [fore_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/fore_ole_color) |  |
| [back_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/back_ole_color) |  |
| [is_visible](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_visible) |  |
| [shadow](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/shadow) |  |
| [linked_cell](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/linked_cell) |  |
| [list_fill_range](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/list_fill_range) |  |
| [data](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/data) |  |
| [is_enabled](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_enabled) |  |
| [is_locked](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_locked) |  |
| [is_transparent](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_transparent) |  |
| [is_auto_size](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/is_auto_size) |  |
| [ime_mode](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/ime_mode) |  |
| [font](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/font) |  |
| [text_align](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/text_align) |  |
| [min](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min) | Gets and sets the minimum acceptable value. |
| [max](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max) | Gets and sets the maximum acceptable value. |
| [position](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position) | Gets and sets the value. |
| [small_change](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/small_change) | Gets and sets the amount by which the Position property changes |
| [orientation](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation) | Gets and sets whether the SpinButton or ScrollBar is oriented vertically or horizontally. |
### Example
```python
from aspose import pycore
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType, SpinButtonActiveXControl
# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.SPIN_BUTTON, 1, 0, 1, 0, 100, 50)
activeXControl = pycore.cast(SpinButtonActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")
```
### See Also
* module [`aspose.cells.drawing.activexcontrols`](..)
* class [`SpinButtonActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)
