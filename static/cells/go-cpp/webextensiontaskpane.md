##WebExtensionTaskPane Class
'WebExtensionTaskPane class. Encapsulates the object that represents webextensiontaskpane in Go.'
## WebExtensionTaskPane class
Represents a persisted taskpane object.
```go
type WebExtensionTaskPane struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetWebExtension](./getwebextension/) | Gets and sets the web extension part associated with the taskpane instance |
|[SetWebExtension](./setwebextension/) | Gets and sets the web extension part associated with the taskpane instance |
|[GetDockState](./getdockstate/) | Gets and sets the last-docked location of this taskpane object. |
|[SetDockState](./setdockstate/) | Gets and sets the last-docked location of this taskpane object. |
|[IsVisible](./isvisible/) | Indicates whether the Task Pane shows as visible by default when the document opens. |
|[SetIsVisible](./setisvisible/) | Indicates whether the Task Pane shows as visible by default when the document opens. |
|[IsLocked](./islocked/) | Indicates whether the taskpane is locked to the document in the UI and cannot be closed by the user. |
|[SetIsLocked](./setislocked/) | Indicates whether the taskpane is locked to the document in the UI and cannot be closed by the user. |
|[GetWidth](./getwidth/) | Gets and sets the default width value for this taskpane instance. |
|[SetWidth](./setwidth/) | Gets and sets the default width value for this taskpane instance. |
|[GetRow](./getrow/) | Gets and sets the index, enumerating from the outside to the inside, of this taskpane among other persisted taskpanes docked in the same default location. |
|[SetRow](./setrow/) | Gets and sets the index, enumerating from the outside to the inside, of this taskpane among other persisted taskpanes docked in the same default location. |
