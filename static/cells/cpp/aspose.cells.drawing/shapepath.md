##Aspose::Cells::Drawing::ShapePath class
'Aspose::Cells::Drawing::ShapePath class. Represents a creation path consisting of a series of moves, lines and curves that when combined will form a geometric shape in C++.'
## ShapePath class
Represents a creation path consisting of a series of moves, lines and curves that when combined will form a geometric shape.
```cpp
class ShapePath
```
## Methods
| Method | Description |
| --- | --- |
| [ArcTo(float wR, float hR, float stAng, float swAng)](./arcto/) | Appends an elliptical arc to the current figure. The starting point is the end point of the current figure. |
| [Close()](./close/) | Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves, the method closes the loop by connecting a line from the endpoint to the starting point. |
| [CubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)](./cubicbezierto/) | Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure.Unit: Pixel. |
| [GetHeightPixel()](./getheightpixel/) | Gets the height of this path in unit of pixels. |
| [GetPathSegementList()](./getpathsegementlist/) | Gets [ShapeSegmentPathCollection](../shapesegmentpathcollection/) list. |
| [GetWidthPixel()](./getwidthpixel/) | Gets the width of this path in unit of pixels. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [LineTo(float x, float y)](./lineto/) | Appends a line segment to the current figure. The starting point is the end point of the current figure.Unit: Pixel. |
| [MoveTo(float x, float y)](./moveto/) | Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure.Unit: Pixel. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ShapePath\& src)](./operator_asm/) | operator= |
| [SetHeightPixel(int32_t value)](./setheightpixel/) | Gets the height of this path in unit of pixels. |
| [SetWidthPixel(int32_t value)](./setwidthpixel/) | Gets the width of this path in unit of pixels. |
| [ShapePath()](./shapepath/) | Initializes a new instance of the [ShapePath](./) class. |
| [ShapePath(ShapePath_Impl* impl)](./shapepath/) | Constructs from an implementation object. |
| [ShapePath(const ShapePath\& src)](./shapepath/) | Copy constructor. |
| [~ShapePath()](./~shapepath/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
