##ShapePathType
Represents path segment type.
## ShapePathType enumeration
Represents path segment type.
### Values
| Name | Value | Description |
| --- | --- | --- |
| LineTo | `1` | Straight line segment |
| CubicBezierCurveTo | `3` | Cubic Bezier curve |
| MoveTo | `0` | Start a new path |
| Close | `128` | If the starting POINT and the end POINT are not the same, a single straight line is drawn to connect the starting POINT and ending POINT of the path. |
| End | `4` | The end of the current path |
| Escape | `5` | Escape |
| ArcTo | `6` | An arc |
| Unknown | `7` | Unknown |
