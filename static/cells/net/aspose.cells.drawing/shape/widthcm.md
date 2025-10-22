##Shape.WidthCM
Shape property. Represents the width of the shape in unit of centimeters
## Shape.WidthCM property
Represents the width of the shape, in unit of centimeters.
```csharp
public double WidthCM { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyWidthCMDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 100, 100);
// Set width in centimeters
shape.WidthCM = 3.5;
Console.WriteLine("Shape width set to: " + shape.WidthCM + " cm");
// Modify width if it matches a condition
if (shape.WidthCM == 3.5)
{
shape.WidthCM = 2.0;
Console.WriteLine("Shape width changed to: " + shape.WidthCM + " cm");
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
