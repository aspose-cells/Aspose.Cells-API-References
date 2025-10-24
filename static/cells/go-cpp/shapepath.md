##ShapePath Class
'ShapePath class. Encapsulates the object that represents shapepath in Go.'
## ShapePath class
Represents a creation path consisting of a series of moves, lines and curves that when combined will form a geometric shape.
```go
type ShapePath struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewShapePath](./newshapepath/) | Initializes a new instance of the ShapePath class. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetPathSegementList](./getpathsegementlist/) | Gets ShapeSegmentPathCollection list |
|[GetWidthPixel](./getwidthpixel/) | Gets the width of this path in unit of pixels. |
|[SetWidthPixel](./setwidthpixel/) | Gets the width of this path in unit of pixels. |
|[GetHeightPixel](./getheightpixel/) | Gets the height of this path in unit of pixels. |
|[SetHeightPixel](./setheightpixel/) | Gets the height of this path in unit of pixels. |
|[MoveTo](./moveto/) | Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure.Unit: Pixel. |
|[LineTo](./lineto/) | Appends a line segment to the current figure.The starting point is the end point of the current figure.Unit: Pixel. |
|[CubicBezierTo](./cubicbezierto/) | Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure.Unit: Pixel. |
|[ArcTo](./arcto/) | Appends an elliptical arc to the current figure. The starting point is the end point of the current figure. |
|[Close](./close/) | Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves, the method closes the loop by connecting a line from the endpoint to the starting point. |
