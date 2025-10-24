##Shape.TopCM
Shape property. Represents the vertical offset of shape from its top row in unit of centimeters
## Shape.TopCM property
Represents the vertical offset of shape from its top row, in unit of centimeters.
```csharp
public double TopCM { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTopCMDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
shape.TopCM = 3.0;
Console.WriteLine("Shape Top position (cm): " + shape.TopCM);
if (shape.TopCM == 3.0)
shape.TopCM = 1.0;
Console.WriteLine("Shape Top position after change (cm): " + shape.TopCM);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
