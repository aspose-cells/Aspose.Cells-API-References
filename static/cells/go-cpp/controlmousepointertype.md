##ControlMousePointerType Enum
'ControlMousePointerType enum. Encapsulates the object that represents controlmousepointertype in Go.'
## ControlMousePointerType Enum
Represents the type of icon displayed as the mouse pointer for the control.
```go
type ControlMousePointerType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Default](./default/) | Standard pointer. |
|[Arrow](./arrow/) | Arrow. |
|[Cross](./cross/) | Cross-hair pointer. |
|[IBeam](./ibeam/) | I-beam. |
|[SizeNESW](./sizenesw/) | Double arrow pointing northeast and southwest. |
|[SizeNS](./sizens/) | Double arrow pointing north and south. |
|[SizeNWSE](./sizenwse/) | Double arrow pointing northwest and southeast. |
|[SizeWE](./sizewe/) | Double arrow pointing west and east. |
|[UpArrow](./uparrow/) | Up arrow. |
|[HourGlass](./hourglass/) | Hourglass. |
|[NoDrop](./nodrop/) | "Not” symbol (circle with a diagonal line) on top of the object being dragged. |
|[AppStarting](./appstarting/) | Arrow with an hourglass. |
|[Help](./help/) | Arrow with a question mark. |
|[SizeAll](./sizeall/) | "Size-all” cursor (arrows pointing north, south, east, and west). |
|[Custom](./custom/) | Uses the icon specified by the MouseIcon property. |
