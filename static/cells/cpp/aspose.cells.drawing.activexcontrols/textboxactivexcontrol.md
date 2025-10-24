##Aspose::Cells::Drawing::ActiveXControls::TextBoxActiveXControl class
'Aspose::Cells::Drawing::ActiveXControls::TextBoxActiveXControl class. Represents a text box ActiveX control in C++.'
## TextBoxActiveXControl class
Represents a text box ActiveX control.
```cpp
class TextBoxActiveXControl : public Aspose::Cells::Drawing::ActiveXControls::ActiveXControl
```
## Methods
| Method | Description |
| --- | --- |
| [ActiveXControl(ActiveXControl_Impl* impl)](../activexcontrol/activexcontrol/) | Constructs from an implementation object. |
| [ActiveXControl(const ActiveXControl\& src)](../activexcontrol/activexcontrol/) | Copy constructor. |
| [ActiveXControl(const ActiveXControlBase\& src)](../activexcontrol/activexcontrol/) | Constructs from a parent object. |
| [ActiveXControlBase(ActiveXControlBase_Impl* impl)](../activexcontrolbase/activexcontrolbase/) | Constructs from an implementation object. |
| [ActiveXControlBase(const ActiveXControlBase\& src)](../activexcontrolbase/activexcontrolbase/) | Copy constructor. |
| [GetBackOleColor()](../activexcontrolbase/getbackolecolor/) | Gets and sets the ole color of the background. |
| [GetBorderOleColor()](./getborderolecolor/) | Gets and sets the ole color of the background. |
| [GetBorderStyle()](./getborderstyle/) | Gets and set the type of border used by the control. |
| [GetData()](../activexcontrol/getdata/) | Gets and sets the binary data of the control. |
| [GetDropButtonStyle()](./getdropbuttonstyle/) | Specifies the symbol displayed on the drop button. |
| [GetEnterFieldBehavior()](./getenterfieldbehavior/) | Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control. |
| [GetEnterKeyBehavior()](./getenterkeybehavior/) | Specifies the behavior of the ENTER key. True specifies that pressing ENTER will create a new line. False specifies that pressing ENTER will move the focus to the next object in the tab order. |
| [GetFont()](../activexcontrol/getfont/) | Represents the font of the control. |
| [GetForeOleColor()](../activexcontrolbase/getforeolecolor/) | Gets and sets the ole color of the foreground. |
| [GetHeight()](../activexcontrolbase/getheight/) | Gets and sets the height of the control in unit of points. |
| [GetHideSelection()](./gethideselection/) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [GetIMEMode()](../activexcontrol/getimemode/) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [GetIntegralHeight()](./getintegralheight/) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
| [GetLinkedCell()](../activexcontrolbase/getlinkedcell/) | Gets and sets the linked cell. |
| [GetListFillRange()](../activexcontrolbase/getlistfillrange/) | Gets and sets the list fill range. |
| [GetMaxLength()](./getmaxlength/) | Gets and sets the maximum number of characters. |
| [GetMouseIcon()](../activexcontrolbase/getmouseicon/) | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [GetMousePointer()](../activexcontrolbase/getmousepointer/) | Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [GetPasswordChar()](./getpasswordchar/) | Gets and sets a character to be displayed in place of the characters entered. |
| [GetScrollBars()](./getscrollbars/) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. |
| [GetShadow()](../activexcontrolbase/getshadow/) | Indicates whether to show a shadow. |
| [GetShowDropButtonTypeWhen()](./getshowdropbuttontypewhen/) | Specifies the symbol displayed on the drop button. |
| [GetSpecialEffect()](./getspecialeffect/) | Gets and sets the special effect of the control. |
| [GetTabKeyBehavior()](./gettabkeybehavior/) | Indicates whether tab characters are allowed in the text of the control. |
| [GetText()](./gettext/) | Gets and set text of the control. |
| [GetTextAlign()](../activexcontrol/gettextalign/) | Represents how to align the text used by the control. |
| virtual [GetType()](./gettype/) | Gets the type of the ActiveX control. |
| [GetWidth()](../activexcontrolbase/getwidth/) | Gets and sets the width of the control in unit of points. |
| [GetWorkbook()](../activexcontrolbase/getworkbook/) | Gets the [Workbook](../../aspose.cells/workbook/) object. |
| [IsAutoSize()](../activexcontrol/isautosize/) | Indicates whether the control will automatically resize to display its entire contents. |
| [IsAutoTab()](./isautotab/) | Indicates whether the focus will automatically move to the next control when the user enters the maximum number of characters. |
| [IsAutoWordSelected()](./isautowordselected/) | Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word. |
| [IsDragBehaviorEnabled()](./isdragbehaviorenabled/) | Indicates whether dragging and dropping is enabled for the control. |
| [IsEditable()](./iseditable/) | Indicates whether the user can type into the control. |
| [IsEnabled()](../activexcontrol/isenabled/) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [IsLocked()](../activexcontrol/islocked/) | Indicates whether data in the control is locked for editing. |
| [IsMultiLine()](./ismultiline/) | Indicates whether the control can display more than one line of text. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsTransparent()](../activexcontrol/istransparent/) | Indicates whether the control is transparent. |
| [IsVisible()](../activexcontrolbase/isvisible/) | Indicates whether this control is visible. |
| [IsWordWrapped()](./iswordwrapped/) | Indicates whether the contents of the control automatically wrap at the end of a line. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const TextBoxActiveXControl\& src)](./operator_asm/) | operator= |
| [operator=(const ActiveXControl\& src)](../activexcontrol/operator_asm/) | operator= |
| [operator=(const ActiveXControlBase\& src)](../activexcontrolbase/operator_asm/) | operator= |
| [SetBackOleColor(int32_t value)](../activexcontrolbase/setbackolecolor/) | Gets and sets the ole color of the background. |
| [SetBorderOleColor(int32_t value)](./setborderolecolor/) | Gets and sets the ole color of the background. |
| [SetBorderStyle(ControlBorderType value)](./setborderstyle/) | Gets and set the type of border used by the control. |
| [SetDropButtonStyle(DropButtonStyle value)](./setdropbuttonstyle/) | Specifies the symbol displayed on the drop button. |
| [SetEnterFieldBehavior(bool value)](./setenterfieldbehavior/) | Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control. |
| [SetEnterKeyBehavior(bool value)](./setenterkeybehavior/) | Specifies the behavior of the ENTER key. True specifies that pressing ENTER will create a new line. False specifies that pressing ENTER will move the focus to the next object in the tab order. |
| [SetForeOleColor(int32_t value)](../activexcontrolbase/setforeolecolor/) | Gets and sets the ole color of the foreground. |
| [SetHeight(double value)](../activexcontrolbase/setheight/) | Gets and sets the height of the control in unit of points. |
| [SetHideSelection(bool value)](./sethideselection/) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
| [SetIMEMode(InputMethodEditorMode value)](../activexcontrol/setimemode/) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| [SetIntegralHeight(bool value)](./setintegralheight/) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
| [SetIsAutoSize(bool value)](../activexcontrol/setisautosize/) | Indicates whether the control will automatically resize to display its entire contents. |
| [SetIsAutoTab(bool value)](./setisautotab/) | Indicates whether the focus will automatically move to the next control when the user enters the maximum number of characters. |
| [SetIsAutoWordSelected(bool value)](./setisautowordselected/) | Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word. |
| [SetIsDragBehaviorEnabled(bool value)](./setisdragbehaviorenabled/) | Indicates whether dragging and dropping is enabled for the control. |
| [SetIsEditable(bool value)](./setiseditable/) | Indicates whether the user can type into the control. |
| [SetIsEnabled(bool value)](../activexcontrol/setisenabled/) | Indicates whether the control can receive the focus and respond to user-generated events. |
| [SetIsLocked(bool value)](../activexcontrol/setislocked/) | Indicates whether data in the control is locked for editing. |
| [SetIsMultiLine(bool value)](./setismultiline/) | Indicates whether the control can display more than one line of text. |
| [SetIsTransparent(bool value)](../activexcontrol/setistransparent/) | Indicates whether the control is transparent. |
| [SetIsVisible(bool value)](../activexcontrolbase/setisvisible/) | Indicates whether this control is visible. |
| [SetIsWordWrapped(bool value)](./setiswordwrapped/) | Indicates whether the contents of the control automatically wrap at the end of a line. |
| [SetLinkedCell(const U16String\& value)](../activexcontrolbase/setlinkedcell/) | Gets and sets the linked cell. |
| [SetLinkedCell(const char16_t* value)](../activexcontrolbase/setlinkedcell/) | Gets and sets the linked cell. |
| [SetListFillRange(const U16String\& value)](../activexcontrolbase/setlistfillrange/) | Gets and sets the list fill range. |
| [SetListFillRange(const char16_t* value)](../activexcontrolbase/setlistfillrange/) | Gets and sets the list fill range. |
| [SetMaxLength(int32_t value)](./setmaxlength/) | Gets and sets the maximum number of characters. |
| [SetMouseIcon(const Vector \<uint8_t\>\& value)](../activexcontrolbase/setmouseicon/) | Gets and sets a custom icon to display as the mouse pointer for the control. |
| [SetMousePointer(ControlMousePointerType value)](../activexcontrolbase/setmousepointer/) | Gets and sets the type of icon displayed as the mouse pointer for the control. |
| [SetPasswordChar(char16_t value)](./setpasswordchar/) | Gets and sets a character to be displayed in place of the characters entered. |
| [SetScrollBars(ControlScrollBarType value)](./setscrollbars/) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. |
| [SetShadow(bool value)](../activexcontrolbase/setshadow/) | Indicates whether to show a shadow. |
| [SetShowDropButtonTypeWhen(ShowDropButtonType value)](./setshowdropbuttontypewhen/) | Specifies the symbol displayed on the drop button. |
| [SetSpecialEffect(ControlSpecialEffectType value)](./setspecialeffect/) | Gets and sets the special effect of the control. |
| [SetTabKeyBehavior(bool value)](./settabkeybehavior/) | Indicates whether tab characters are allowed in the text of the control. |
| [SetText(const U16String\& value)](./settext/) | Gets and set text of the control. |
| [SetText(const char16_t* value)](./settext/) | Gets and set text of the control. |
| [SetTextAlign(TextAlignmentType value)](../activexcontrol/settextalign/) | Represents how to align the text used by the control. |
| [SetWidth(double value)](../activexcontrolbase/setwidth/) | Gets and sets the width of the control in unit of points. |
| [TextBoxActiveXControl(TextBoxActiveXControl_Impl* impl)](./textboxactivexcontrol/) | Constructs from an implementation object. |
| [TextBoxActiveXControl(const TextBoxActiveXControl\& src)](./textboxactivexcontrol/) | Copy constructor. |
| [TextBoxActiveXControl(const ActiveXControl\& src)](./textboxactivexcontrol/) | Constructs from a parent object. |
| [~ActiveXControl()](../activexcontrol/~activexcontrol/) | Destructor. |
| [~ActiveXControlBase()](../activexcontrolbase/~activexcontrolbase/) | Destructor. |
| [~TextBoxActiveXControl()](./~textboxactivexcontrol/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Initialize a new workbook.
Workbook book;
//Add a TextBoxActiveXControl.
Shape shape = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl(ControlType::TextBox, 1, 0, 1, 0, 100, 50);
TextBoxActiveXControl activeXControl = (TextBoxActiveXControl)shape.GetActiveXControl();
//Save the excel file.
book.Save(u"exmaple.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Class [ActiveXControl](../activexcontrol/)
* Namespace [Aspose::Cells::Drawing::ActiveXControls](../)
* Library [Aspose.Cells for C++](../../)
