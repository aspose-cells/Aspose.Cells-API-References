##Shape.HeightCM
Shape property. Represents the height of the shape in unit of centimeters
## Shape.HeightCM property
Represents the height of the shape, in unit of centimeters.
```csharp
public double HeightCM { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyHeightCMDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
// Set height in centimeters
shape.HeightCM = 3;
Console.WriteLine("Shape height: " + shape.HeightCM + " cm");
// Modify height if it's 3 cm
if (shape.HeightCM == 3)
{
shape.HeightCM = 1;
Console.WriteLine("Modified shape height: " + shape.HeightCM + " cm");
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
