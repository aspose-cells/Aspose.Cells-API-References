##Aspose::Cells::Drawing::ShapePathType enum
'Aspose::Cells::Drawing::ShapePathType enum. Represents path segment type in C++.'
## ShapePathType enum
Represents path segment type.
```cpp
enum class ShapePathType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| LineTo | 1 | <br>Straight line segment. |
| CubicBezierCurveTo | 3 | <br>Cubic Bezier curve. |
| MoveTo | 0 | <br>Start a new path. |
| Close | 128 | <br>If the starting POINT and the end POINT are not the same, a single straight line is drawn to connect the starting POINT and ending POINT of the path. |
| End | 4 | <br>The end of the current path. |
| Escape | 5 | <br>Escape. |
| ArcTo | 6 | <br>An arc. |
| Unknown | 7 | <br>Unknown. |
## See Also
* Namespace [Aspose::Cells::Drawing](../)
* Library [Aspose.Cells for C++](../../)
