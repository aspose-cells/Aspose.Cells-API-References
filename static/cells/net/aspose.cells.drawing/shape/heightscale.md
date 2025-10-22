##Shape.HeightScale
Shape property. Gets and sets the height scalein unit of percent of the original picture height. If the shape is not picture the HeightScale property only returns 100
## Shape.HeightScale property
Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;
```csharp
public int HeightScale { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyHeightScaleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 150);
// Set initial height scale
shape.HeightScale = 50;
Console.WriteLine("Initial HeightScale: " + shape.HeightScale);
// Modify height scale if condition is met
if (shape.HeightScale == 50)
{
shape.HeightScale = 75;
Console.WriteLine("Modified HeightScale: " + shape.HeightScale);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
