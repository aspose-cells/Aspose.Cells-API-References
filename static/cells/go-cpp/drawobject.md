##DrawObject Class
'DrawObject class. Encapsulates the object that represents drawobject in Go.'
## DrawObject class
DrawObject will be initialized and returned when rendering.
```go
type DrawObject struct  {
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
|[GetCell](./getcell/) | Indicates the Cell object when rendering.All properties of cell can be accessed. |
|[GetShape](./getshape/) | Indicates the Shape object when rendering.All properties of shape can be accessed. |
|[GetImageBytes](./getimagebytes/) | Indicates image bytes of rendered Chart, Shape when rendering. |
|[GetType](./gettype/) | Indicates the type of DrawObject. |
|[GetCurrentPage](./getcurrentpage/) | Indicates the page index of DrawObject.Page index is based on zero.One Sheet contains several pages when rendering. |
|[GetTotalPages](./gettotalpages/) | Indicates total pages in current rendering. |
|[GetSheetIndex](./getsheetindex/) | Indicates current sheet index of DrawObject. |
