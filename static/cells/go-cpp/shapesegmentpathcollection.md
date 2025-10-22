##ShapeSegmentPathCollection Class
'ShapeSegmentPathCollection class. Encapsulates the object that represents shapesegmentpathcollection in Go.'
## ShapeSegmentPathCollection class
Represents a creation path consisting of a series of moves, lines and curves that when combined will form a geometric shape.
```go
type ShapeSegmentPathCollection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewShapeSegmentPathCollection](./newshapesegmentpathcollection/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[Add](./add/) | Add a segment path in creation path. |
|[Get](./get/) | Gets ShapeSegmentPath object. |
|[GetCount](./getcount/) |  |
