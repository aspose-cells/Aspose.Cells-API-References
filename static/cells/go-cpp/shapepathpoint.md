##ShapePathPoint Class
'ShapePathPoint class. Encapsulates the object that represents shapepathpoint in Go.'
## ShapePathPoint class
Specify position coordinates or angle markers.Position coordinates represent the coordinates of a path in a coordinate space (e.g. X/Y).Angle markers indicate angular changes in a path (e.g. the start and swing angles of an arc).
```go
type ShapePathPoint struct  {
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
|[GetXPixel](./getxpixel/) | When the object is a position coordinate, get or set the x coordinate in pixels. |
|[SetXPixel](./setxpixel/) | When the object is a position coordinate, get or set the x coordinate in pixels. |
|[GetYPixel](./getypixel/) | When the object is a position coordinate, get or set the y coordinate in pixels. |
|[SetYPixel](./setypixel/) | When the object is a position coordinate, get or set the y coordinate in pixels. |
|[GetXAngle](./getxangle/) | When the object is an angle marker, get or set the first angle in degrees. |
|[SetXAngle](./setxangle/) | When the object is an angle marker, get or set the first angle in degrees. |
|[GetYAngle](./getyangle/) | When the object is an angle marker, get or set the second angle in degrees. |
|[SetYAngle](./setyangle/) | When the object is an angle marker, get or set the second angle in degrees. |
|[GetType](./gettype/) | Specifies the value type of the current object. |
