##Shape.HasLine
Shape property. Gets and sets the line border of the shape is visible
## Shape.HasLine property
Gets and sets the line border of the shape is visible.
```csharp
public bool HasLine { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyHasLineDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
// Demonstrate HasLine property
Console.WriteLine("Shape initially has line: " + shape.HasLine);
// Remove the line
shape.HasLine = false;
Console.WriteLine("After setting HasLine to false: " + shape.HasLine);
// Add the line back
shape.HasLine = true;
Console.WriteLine("After setting HasLine to true: " + shape.HasLine);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
