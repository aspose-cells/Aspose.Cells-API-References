##Shape.TopInch
Shape property. Represents the vertical offset of shape from its top row in unit of inches
## Shape.TopInch property
Represents the vertical offset of shape from its top row, in unit of inches.
```csharp
public double TopInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTopInchDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
// Set and demonstrate TopInch property
shape.TopInch = 3;
Console.WriteLine("Shape Top position (inches): " + shape.TopInch);
// Modify TopInch if it equals 3
if (shape.TopInch == 3)
{
shape.TopInch = 1;
Console.WriteLine("Modified Shape Top position (inches): " + shape.TopInch);
}
// Save the workbook
workbook.Save("ShapeTopInchDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
