##TextBoxActiveXControl Class
'TextBoxActiveXControl class. Encapsulates the object that represents textboxactivexcontrol in Go.'
## TextBoxActiveXControl class
Represents a text box ActiveX control.
```go
type TextBoxActiveXControl struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewTextBoxActiveXControl](./newtextboxactivexcontrol/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Gets the type of the ActiveX control. |
|[GetBorderStyle](./getborderstyle/) | Gets and set the type of border used by the control. |
|[SetBorderStyle](./setborderstyle/) | Gets and set the type of border used by the control. |
|[GetBorderOleColor](./getborderolecolor/) | Gets and sets the ole color of the background. |
|[SetBorderOleColor](./setborderolecolor/) | Gets and sets the ole color of the background. |
|[GetSpecialEffect](./getspecialeffect/) | Gets and sets the special effect of the control. |
|[SetSpecialEffect](./setspecialeffect/) | Gets and sets the special effect of the control. |
|[GetMaxLength](./getmaxlength/) | Gets and sets the maximum number of characters |
|[SetMaxLength](./setmaxlength/) | Gets and sets the maximum number of characters |
|[GetScrollBars](./getscrollbars/) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. |
|[SetScrollBars](./setscrollbars/) | Indicates specifies whether the control has vertical scroll bars, horizontal scroll bars, both, or neither. |
|[GetPasswordChar](./getpasswordchar/) | Gets and sets a character to be displayed in place of the characters entered. |
|[SetPasswordChar](./setpasswordchar/) | Gets and sets a character to be displayed in place of the characters entered. |
|[IsEditable](./iseditable/) | Indicates whether the user can type into the control. |
|[SetIsEditable](./setiseditable/) | Indicates whether the user can type into the control. |
|[GetIntegralHeight](./getintegralheight/) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
|[SetIntegralHeight](./setintegralheight/) | Indicates whether the control will only show complete lines of text without showing any partial lines. |
|[IsDragBehaviorEnabled](./isdragbehaviorenabled/) | Indicates whether dragging and dropping is enabled for the control. |
|[SetIsDragBehaviorEnabled](./setisdragbehaviorenabled/) | Indicates whether dragging and dropping is enabled for the control. |
|[GetEnterKeyBehavior](./getenterkeybehavior/) | Specifies the behavior of the ENTER key.True specifies that pressing ENTER will create a new line.False specifies that pressing ENTER will move the focus to the next object in the tab order. |
|[SetEnterKeyBehavior](./setenterkeybehavior/) | Specifies the behavior of the ENTER key.True specifies that pressing ENTER will create a new line.False specifies that pressing ENTER will move the focus to the next object in the tab order. |
|[GetEnterFieldBehavior](./getenterfieldbehavior/) | Specifies selection behavior when entering the control.True specifies that the selection remains unchanged from last time the control was active.False specifies that all the text in the control will be selected when entering the control. |
|[SetEnterFieldBehavior](./setenterfieldbehavior/) | Specifies selection behavior when entering the control.True specifies that the selection remains unchanged from last time the control was active.False specifies that all the text in the control will be selected when entering the control. |
|[GetTabKeyBehavior](./gettabkeybehavior/) | Indicates whether tab characters are allowed in the text of the control. |
|[SetTabKeyBehavior](./settabkeybehavior/) | Indicates whether tab characters are allowed in the text of the control. |
|[GetHideSelection](./gethideselection/) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
|[SetHideSelection](./sethideselection/) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
|[IsAutoTab](./isautotab/) | Indicates whether the focus will automatically move to the next control when the user enters the maximum number of characters. |
|[SetIsAutoTab](./setisautotab/) | Indicates whether the focus will automatically move to the next control when the user enters the maximum number of characters. |
|[IsMultiLine](./ismultiline/) | Indicates whether the control can display more than one line of text. |
|[SetIsMultiLine](./setismultiline/) | Indicates whether the control can display more than one line of text. |
|[IsWordWrapped](./iswordwrapped/) | Indicates whether the contents of the control automatically wrap at the end of a line. |
|[SetIsWordWrapped](./setiswordwrapped/) | Indicates whether the contents of the control automatically wrap at the end of a line. |
|[GetText](./gettext/) | Gets and set text of the control. |
|[SetText](./settext/) | Gets and set text of the control. |
|[GetDropButtonStyle](./getdropbuttonstyle/) | Specifies the symbol displayed on the drop button |
|[SetDropButtonStyle](./setdropbuttonstyle/) | Specifies the symbol displayed on the drop button |
|[GetShowDropButtonTypeWhen](./getshowdropbuttontypewhen/) | Specifies the symbol displayed on the drop button |
|[SetShowDropButtonTypeWhen](./setshowdropbuttontypewhen/) | Specifies the symbol displayed on the drop button |
|[IsAutoWordSelected](./isautowordselected/) | Specifies the basic unit used to extend a selection.True specifies that the basic unit is a single character.false specifies that the basic unit is a whole word. |
|[SetIsAutoWordSelected](./setisautowordselected/) | Specifies the basic unit used to extend a selection.True specifies that the basic unit is a single character.false specifies that the basic unit is a whole word. |
|[IsEnabled](./isenabled/) | Indicates whether the control can receive the focus and respond to user-generated events. |
|[SetIsEnabled](./setisenabled/) | Indicates whether the control can receive the focus and respond to user-generated events. |
|[IsLocked](./islocked/) | Indicates whether data in the control is locked for editing. |
|[SetIsLocked](./setislocked/) | Indicates whether data in the control is locked for editing. |
|[IsTransparent](./istransparent/) | Indicates whether the control is transparent. |
|[SetIsTransparent](./setistransparent/) | Indicates whether the control is transparent. |
|[GetIMEMode](./getimemode/) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
|[SetIMEMode](./setimemode/) | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
|[GetFont](./getfont/) | Represents the font of the control. |
|[GetTextAlign](./gettextalign/) | Represents how to align the text used by the control. |
|[SetTextAlign](./settextalign/) | Represents how to align the text used by the control. |
|[GetData](./getdata/) | Gets and sets the binary data of the control. |
|[IsAutoSize](./isautosize/) | Indicates whether the control will automatically resize to display its entire contents. |
|[SetIsAutoSize](./setisautosize/) | Indicates whether the control will automatically resize to display its entire contents. |
|[GetWorkbook](./getworkbook/) | Gets the Workbook object. |
|[GetMouseIcon](./getmouseicon/) | Gets and sets a custom icon to display as the mouse pointer for the control. |
|[SetMouseIcon](./setmouseicon/) | Gets and sets a custom icon to display as the mouse pointer for the control. |
|[GetMousePointer](./getmousepointer/) | Gets and sets the type of icon displayed as the mouse pointer for the control. |
|[SetMousePointer](./setmousepointer/) | Gets and sets the type of icon displayed as the mouse pointer for the control. |
|[GetLinkedCell](./getlinkedcell/) | Gets and sets the linked cell. |
|[SetLinkedCell](./setlinkedcell/) | Gets and sets the linked cell. |
|[GetListFillRange](./getlistfillrange/) | Gets and sets the list fill range. |
|[SetListFillRange](./setlistfillrange/) | Gets and sets the list fill range. |
|[GetWidth](./getwidth/) | Gets and sets the width of the control in unit of points. |
|[SetWidth](./setwidth/) | Gets and sets the width of the control in unit of points. |
|[GetHeight](./getheight/) | Gets and sets the height of the control in unit of points. |
|[SetHeight](./setheight/) | Gets and sets the height of the control in unit of points. |
|[GetForeOleColor](./getforeolecolor/) | Gets and sets the ole color of the foreground. |
|[SetForeOleColor](./setforeolecolor/) | Gets and sets the ole color of the foreground. |
|[GetBackOleColor](./getbackolecolor/) | Gets and sets the ole color of the background. |
|[SetBackOleColor](./setbackolecolor/) | Gets and sets the ole color of the background. |
|[IsVisible](./isvisible/) | Indicates whether this control is visible. |
|[SetIsVisible](./setisvisible/) | Indicates whether this control is visible. |
|[GetShadow](./getshadow/) | Indicates whether to show a shadow. |
|[SetShadow](./setshadow/) | Indicates whether to show a shadow. |
