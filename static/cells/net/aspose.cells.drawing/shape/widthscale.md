##Shape.WidthScale
Shape property. Gets and sets the width scale in unit of percent of the original picture width. If the shape is not picture the WidthScale property only returns 100
## Shape.WidthScale property
Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;
```csharp
public int WidthScale { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyWidthScaleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with correct parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
// Set initial width scale
shape.WidthScale = 50;
Console.WriteLine("Initial WidthScale: " + shape.WidthScale);
// Modify width scale if condition is met
if (shape.WidthScale == 50)
{
shape.WidthScale = 75;
Console.WriteLine("Updated WidthScale: " + shape.WidthScale);
}
// Save the workbook
workbook.Save("ShapeWidthScaleDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
