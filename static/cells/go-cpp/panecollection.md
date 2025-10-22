##PaneCollection Class
'PaneCollection class. Encapsulates the object that represents panecollection in Go.'
## PaneCollection class
Represents all Pane objects shown in the specified window.
```go
type PaneCollection struct  {
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
|[GetFirstVisibleRowOfBottomPane](./getfirstvisiblerowofbottompane/) | Gets and sets the first visible row of the bottom pane. |
|[SetFirstVisibleRowOfBottomPane](./setfirstvisiblerowofbottompane/) | Gets and sets the first visible row of the bottom pane. |
|[GetFirstVisibleColumnOfRightPane](./getfirstvisiblecolumnofrightpane/) | Gets and sets the first visible column of the right pane. |
|[SetFirstVisibleColumnOfRightPane](./setfirstvisiblecolumnofrightpane/) | Gets and sets the first visible column of the right pane. |
|[GetAcitvePaneType](./getacitvepanetype/) | Gets and sets the active pane. |
|[SetAcitvePaneType](./setacitvepanetype/) | Gets and sets the active pane. |
