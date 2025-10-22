##Shape.IsEquation
Shape property. Indicates whether the shape only contains an equation
## Shape.IsEquation property
Indicates whether the shape only contains an equation.
```csharp
public bool IsEquation { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsEquationDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an equation shape with correct parameters
Shape equationShape = worksheet.Shapes.AddEquation(0, 0, 0, 0, 100, 100);
equationShape.AlternativeText = "x^2 + y^2 = r^2";
// Add a regular rectangle shape with correct parameters
Shape rectangleShape = worksheet.Shapes.AddRectangle(2, 0, 0, 0, 100, 100);
foreach (Shape shape in worksheet.Shapes)
{
if (shape.IsEquation)
{
Console.WriteLine("Shape is an equation: " + shape.AlternativeText);
}
else
{
Console.WriteLine("Shape is not an equation");
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
