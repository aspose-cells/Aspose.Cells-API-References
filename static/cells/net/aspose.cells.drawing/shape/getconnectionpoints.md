##Shape.GetConnectionPoints
Shape method. Get the connection points
## Shape.GetConnectionPoints method
Get the connection points
```csharp
public float[][] GetConnectionPoints()
```
### Return Value
[X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodGetConnectionPointsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
// Get connection points of the shape
float[][] points = shape.GetConnectionPoints();
// Output the connection points
Console.WriteLine("Connection Points:");
for (int i = 0; i < points.Length; i++)
{
Console.WriteLine($"Point {i + 1}: X={points[i][0]}, Y={points[i][1]}");
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
