##ShapeTextAlignment.RotateTextWithShape
ShapeTextAlignment property. Indicates whether rotating text with shape
## ShapeTextAlignment.RotateTextWithShape property
Indicates whether rotating text with shape.
```csharp
public bool RotateTextWithShape { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyRotateTextWithShapeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape with correct parameters
Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
shape.Text = "Sample Text";
// Access text alignment properties
ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
// Set RotateTextWithShape property
textAlignment.RotateTextWithShape = true;
// Rotate the shape to demonstrate the effect
shape.RotationAngle = 45;
// Save the workbook
workbook.Save("RotateTextWithShapeDemo.xlsx");
}
}
}
```
### See Also
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
