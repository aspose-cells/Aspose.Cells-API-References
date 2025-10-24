##Shape.AlternativeText
Shape property. Returns or sets the descriptive alternative text string of the Shape object
## Shape.AlternativeText property
Returns or sets the descriptive (alternative) text string of the [`Shape`](../) object.
```csharp
public string AlternativeText { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyAlternativeTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
// Set alternative text for the shape
shape.AlternativeText = "A rectangle shape with width 100 and height 200";
// Save the workbook
workbook.Save("ShapeAlternativeTextDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
