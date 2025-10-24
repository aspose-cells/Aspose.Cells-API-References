##Shape.TopInShape
Shape property. Represents the vertical offset of shape from the top border of the parent shape in unit of 1/4000 of height of the parent shape
## Shape.TopInShape property
Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.
```csharp
public int TopInShape { get; set; }
```
### Remarks
Only Applies when this shape in the group or chart.
### Examples
```csharp
[C#]
if (shape.IsInGroup && shape.TopInShape == 8000)
shape.TopInShape = 4000;
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
