##ComboBoxActiveXControl Class
'ComboBoxActiveXControl class. Encapsulates the object that represents comboboxactivexcontrol in Go.'
## ComboBoxActiveXControl class
Represents a ComboBox ActiveX control.
```go
type ComboBoxActiveXControl struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewComboBoxActiveXControl](./newcomboboxactivexcontrol/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Gets the type of the ActiveX control. |
|[GetMaxLength](./getmaxlength/) | Gets and sets the maximum number of characters |
|[SetMaxLength](./setmaxlength/) | Gets and sets the maximum number of characters |
|[GetListWidth](./getlistwidth/) | Gets and set the width in unit of points. |
|[SetListWidth](./setlistwidth/) | Gets and set the width in unit of points. |
|[GetBoundColumn](./getboundcolumn/) | Represents how the Value property is determined for a ComboBox or ListBoxwhen the MultiSelect properties value (fmMultiSelectSingle). |
|[SetBoundColumn](./setboundcolumn/) | Represents how the Value property is determined for a ComboBox or ListBoxwhen the MultiSelect properties value (fmMultiSelectSingle). |
|[GetTextColumn](./gettextcolumn/) | Represents the column in a ComboBox or ListBox to display to the user. |
|[SetTextColumn](./settextcolumn/) | Represents the column in a ComboBox or ListBox to display to the user. |
|[GetColumnCount](./getcolumncount/) | Represents the number of columns to display in a ComboBox or ListBox. |
|[SetColumnCount](./setcolumncount/) | Represents the number of columns to display in a ComboBox or ListBox. |
|[GetListRows](./getlistrows/) | Represents the maximum number of rows to display in the list. |
|[SetListRows](./setlistrows/) | Represents the maximum number of rows to display in the list. |
|[GetMatchEntry](./getmatchentry/) | Indicates how a ListBox or ComboBox searches its list as the user types. |
|[SetMatchEntry](./setmatchentry/) | Indicates how a ListBox or ComboBox searches its list as the user types. |
|[GetDropButtonStyle](./getdropbuttonstyle/) | Specifies the symbol displayed on the drop button |
|[SetDropButtonStyle](./setdropbuttonstyle/) | Specifies the symbol displayed on the drop button |
|[GetShowDropButtonTypeWhen](./getshowdropbuttontypewhen/) | Specifies the symbol displayed on the drop button |
|[SetShowDropButtonTypeWhen](./setshowdropbuttontypewhen/) | Specifies the symbol displayed on the drop button |
|[GetListStyle](./getliststyle/) | Gets and sets the visual appearance. |
|[SetListStyle](./setliststyle/) | Gets and sets the visual appearance. |
|[GetBorderStyle](./getborderstyle/) | Gets and set the type of border used by the control. |
|[SetBorderStyle](./setborderstyle/) | Gets and set the type of border used by the control. |
|[GetBorderOleColor](./getborderolecolor/) | Gets and sets the ole color of the background. |
|[SetBorderOleColor](./setborderolecolor/) | Gets and sets the ole color of the background. |
|[GetSpecialEffect](./getspecialeffect/) | Gets and sets the special effect of the control. |
|[SetSpecialEffect](./setspecialeffect/) | Gets and sets the special effect of the control. |
|[IsEditable](./iseditable/) | Indicates whether the user can type into the control. |
|[SetIsEditable](./setiseditable/) | Indicates whether the user can type into the control. |
|[GetShowColumnHeads](./getshowcolumnheads/) | Indicates whether column headings are displayed. |
|[SetShowColumnHeads](./setshowcolumnheads/) | Indicates whether column headings are displayed. |
|[IsDragBehaviorEnabled](./isdragbehaviorenabled/) | Indicates whether dragging and dropping is enabled for the control. |
|[SetIsDragBehaviorEnabled](./setisdragbehaviorenabled/) | Indicates whether dragging and dropping is enabled for the control. |
|[GetEnterFieldBehavior](./getenterfieldbehavior/) | Specifies selection behavior when entering the control.True specifies that the selection remains unchanged from last time the control was active.False specifies that all the text in the control will be selected when entering the control. |
|[SetEnterFieldBehavior](./setenterfieldbehavior/) | Specifies selection behavior when entering the control.True specifies that the selection remains unchanged from last time the control was active.False specifies that all the text in the control will be selected when entering the control. |
|[GetSelectionMargin](./getselectionmargin/) | Indicates whether the user can select a line of text by clicking in the region to the left of the text. |
|[SetSelectionMargin](./setselectionmargin/) | Indicates whether the user can select a line of text by clicking in the region to the left of the text. |
|[GetValue](./getvalue/) | Gets and sets the value of the control. |
|[SetValue](./setvalue/) | Gets and sets the value of the control. |
|[GetHideSelection](./gethideselection/) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
|[SetHideSelection](./sethideselection/) | Indicates whether selected text in the control appears highlighted when the control does not have focus. |
|[GetColumnWidths](./getcolumnwidths/) | Gets and sets the width of the column. |
|[SetColumnWidths](./setcolumnwidths/) | Gets and sets the width of the column. |
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
