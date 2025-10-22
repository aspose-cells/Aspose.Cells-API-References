##Shape.LeftInShape
Shape property. Represents the horizontal offset of shape from the left border of the parent shape in unit of 1/4000 of width of the parent shape
## Shape.LeftInShape property
Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape.
```csharp
public int LeftInShape { get; set; }
```
### Remarks
Only Applies when this shape in the group or chart.
### Examples
```csharp
[C#]
if (shape.IsInGroup && shape.LeftInShape == 2000)
shape.LeftInShape = 4000;
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
