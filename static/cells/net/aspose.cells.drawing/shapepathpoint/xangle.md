##ShapePathPoint.XAngle
ShapePathPoint property. When the object is an angle marker get or set the first angle in degrees
## ShapePathPoint.XAngle property
When the object is an angle marker, get or set the first angle in degrees.
```csharp
public int XAngle { get; set; }
```
### Remarks
If this angle is the starting angle of an arc. This angle will specify what angle along the supposed circle path will be used as the start position for drawing the arc. This start angle will be locked to the last known pen position in the shape path. Thus guaranteeing a continuos shape path.
### See Also
* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
