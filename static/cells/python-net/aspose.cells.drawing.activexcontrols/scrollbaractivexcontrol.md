##ScrollBarActiveXControl class
## ScrollBarActiveXControl class
Represents the ScrollBar control.
**Inheritance:** [`ScrollBarActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol) →
[`SpinButtonActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)
The ScrollBarActiveXControl type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [workbook](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/workbook) |  |
| [type](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/type) | Gets the type of the ActiveX control. |
| [width](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/width) |  |
| [height](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/height) |  |
| [mouse_icon](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/mouse_icon) |  |
| [mouse_pointer](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/mouse_pointer) |  |
| [fore_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/fore_ole_color) |  |
| [back_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/back_ole_color) |  |
| [is_visible](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_visible) |  |
| [shadow](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/shadow) |  |
| [linked_cell](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/linked_cell) |  |
| [list_fill_range](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/list_fill_range) |  |
| [data](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/data) |  |
| [is_enabled](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_enabled) |  |
| [is_locked](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_locked) |  |
| [is_transparent](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_transparent) |  |
| [is_auto_size](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_auto_size) |  |
| [ime_mode](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/ime_mode) |  |
| [font](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/font) |  |
| [text_align](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/text_align) |  |
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
* module [`aspose.cells.drawing.activexcontrols`](..)
* class [`ScrollBarActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol)
* class [`SpinButtonActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)
