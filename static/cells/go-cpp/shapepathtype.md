##ShapePathType Enum
'ShapePathType enum. Encapsulates the object that represents shapepathtype in Go.'
## ShapePathType Enum
Represents path segment type.
```go
type ShapePathType int32
```
## Fields
| Field | Description |
| --- | --- |
|[LineTo](./lineto/) | Straight line segment |
|[CubicBezierCurveTo](./cubicbeziercurveto/) | Cubic Bezier curve |
|[MoveTo](./moveto/) | Start a new path |
|[Close](./close/) | If the starting POINT and the end POINT are not the same, a singlestraight line is drawn to connect the starting POINT and ending POINT of the path. |
|[End](./end/) | The end of the current path |
|[Escape](./escape/) | Escape |
|[ArcTo](./arcto/) | An arc |
|[Unknown](./unknown/) | Unknown |
