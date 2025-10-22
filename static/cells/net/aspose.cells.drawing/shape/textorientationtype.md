##Shape.TextOrientationType
Shape property. Gets and sets the text orientation type of the shape
## Shape.TextOrientationType property
Gets and sets the text orientation type of the shape.
```csharp
public TextOrientationType TextOrientationType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTextOrientationTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);
// Set text for the shape
shape.Text = "Sample Text";
// Check and modify text orientation
if (shape.TextOrientationType == TextOrientationType.NoRotation)
{
shape.TextOrientationType = TextOrientationType.TopToBottom;
}
// Save the workbook
workbook.Save("ShapeTextOrientationDemo.xlsx");
}
}
}
```
### See Also
* enum [TextOrientationType](../../../aspose.cells/textorientationtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
