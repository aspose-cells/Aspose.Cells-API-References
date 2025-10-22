##TextBoxActiveXControl class
## TextBoxActiveXControl class
Represents a text box ActiveX control.
**Inheritance:** [`TextBoxActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol)
The TextBoxActiveXControl type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [workbook](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/workbook) |  |
| [type](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/type) | Gets the type of the ActiveX control. |
| [width](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/width) |  |
| [height](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/height) |  |
| [mouse_icon](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/mouse_icon) |  |
| [mouse_pointer](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/mouse_pointer) |  |
| [fore_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/fore_ole_color) |  |
| [back_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/back_ole_color) |  |
| [is_visible](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/is_visible) |  |
| [shadow](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/shadow) |  |
| [linked_cell](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/linked_cell) |  |
| [list_fill_range](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/list_fill_range) |  |
| [data](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/data) |  |
| [is_enabled](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/is_enabled) |  |
| [is_locked](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/is_locked) |  |
| [is_transparent](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/is_transparent) |  |
| [is_auto_size](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/is_auto_size) |  |
| [ime_mode](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/ime_mode) |  |
| [font](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/font) |  |
| [text_align](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/text_align) |  |
| [border_style](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/border_style) | Gets and set the type of border used by the control. |
| [border_ole_color](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/border_ole_color) | Gets and sets the ole color of the background. |
| [special_effect](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/special_effect) | Gets and sets the special effect of the control. |
| [max_length](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/max_length) | Gets and sets the maximum number of characters |
| [scroll_bars](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/scroll_bars) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. |
| [password_char](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/password_char) | Gets and sets a character to be displayed in place of the characters entered. |
| [is_editable](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/is_editable) | Indicates whether the user can type into the control. |
| [integral_height](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/integral_height) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
| [is_drag_behavior_enabled](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/is_drag_behavior_enabled) | Indicates whether dragging and dropping is enabled for the control. |
| [enter_key_behavior](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enter_key_behavior) | Specifies the behavior of the ENTER key.
| [enter_field_behavior](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enter_field_behavior) | Specifies selection behavior when entering the control.
| [tab_key_behavior](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/tab_key_behavior) | Indicates whether tab characters are allowed in the text of the control. |
| [hide_selection](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/hide_selection) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [is_auto_tab](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/is_auto_tab) | Indicates whether the focus will automatically move to the next control when the user enters the maximum number of characters. |
| [is_multi_line](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/is_multi_line) | Indicates whether the control can display more than one line of text. |
| [is_auto_word_selected](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/is_auto_word_selected) | Specifies the basic unit used to extend a selection.
| [is_word_wrapped](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/is_word_wrapped) | Indicates whether the contents of the control automatically wrap at the end of a line. |
| [text](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/text) | Gets and set text of the control. |
| [drop_button_style](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/drop_button_style) | Specifies the symbol displayed on the drop button |
| [show_drop_button_type_when](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/show_drop_button_type_when) | Specifies the symbol displayed on the drop button |
### Example
```python
from aspose import pycore
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType, TextBoxActiveXControl
# Initialize a new workbook.
book = Workbook()
# Add a TextBoxActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.TEXT_BOX, 1, 0, 1, 0, 100, 50)
activeXControl = pycore.cast(TextBoxActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")
```
### See Also
* module [`aspose.cells.drawing.activexcontrols`](..)
* class [`TextBoxActiveXControl`](/cells/python-net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol)
