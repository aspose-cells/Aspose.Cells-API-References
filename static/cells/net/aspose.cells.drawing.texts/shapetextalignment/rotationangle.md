##ShapeTextAlignment.RotationAngle
ShapeTextAlignment property. Gets and sets the rotation of the shape
## ShapeTextAlignment.RotationAngle property
Gets and sets the rotation of the shape.
```csharp
public double RotationAngle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyRotationAngleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 200, 300, 400);
// Set shape text
shape.Text = "Rotated Text";
// Access text alignment and set rotation angle
shape.TextBody.TextAlignment.RotationAngle = 90;
// Save the workbook
workbook.Save("ShapeTextRotationDemo.xlsx");
}
}
}
```
### See Also
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
