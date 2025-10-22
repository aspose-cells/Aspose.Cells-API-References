##Shape.Top
Shape property. Represents the vertical offset of shape from its top row in unit of pixels
## Shape.Top property
Represents the vertical offset of shape from its top row, in unit of pixels.
```csharp
public int Top { get; set; }
```
### Remarks
If the shape is in the chart, represents the vertical offset of shape from its top border.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTopDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
// Set initial top position
shape.Top = 50;
Console.WriteLine("Initial Top position: " + shape.Top);
// Modify top position if it equals 3 (demonstrating the test case logic)
if (shape.Top == 3)
{
shape.Top = 1;
}
else
{
// For demonstration, set to 3 and then apply the test case logic
shape.Top = 3;
if (shape.Top == 3)
{
shape.Top = 1;
Console.WriteLine("Modified Top position: " + shape.Top);
}
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
