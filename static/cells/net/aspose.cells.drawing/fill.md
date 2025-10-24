##Class Fill
Aspose.Cells.Drawing.Fill class. Represents the fill format of the shape
## Fill class
Represents the fill format of the shape.
```csharp
public abstract class Fill
```
## Methods
| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | / |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Gets the hash code. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
public class DrawingClassFillDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 150);
// Set fill type to solid and modify color
rectangle.Fill.FillType = FillType.Solid;
rectangle.Fill.SolidFill.Color = Color.LightBlue;
Shape oval = worksheet.Shapes.AddOval(2, 0, 0, 0, 100, 150);
// Use gradient fill method directly on FillFormat
oval.Fill.SetTwoColorGradient(Color.DarkBlue, Color.SkyBlue, GradientStyleType.Vertical, 0);
workbook.Save("DrawingClassFillDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
