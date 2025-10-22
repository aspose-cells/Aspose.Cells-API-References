##ActiveXControl Class
'ActiveXControl class. Encapsulates the object that represents activexcontrol in Go.'
## ActiveXControl class
Represents the ActiveX control.
```go
type ActiveXControl struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewActiveXControl](./newactivexcontrol/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
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
|[GetType](./gettype/) | Gets the type of the ActiveX control. |
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
