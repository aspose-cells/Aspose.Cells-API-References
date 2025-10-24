##Shape.Worksheet
Shape property. Gets the Worksheet object which contains this shape
## Shape.Worksheet property
Gets the `Worksheet` object which contains this shape.
```csharp
public Worksheet Worksheet { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyWorksheetDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
// Demonstrate Worksheet property usage
Worksheet shapeWorksheet = shape.Worksheet;
// Output worksheet name to show the property works
Console.WriteLine("Shape belongs to worksheet: " + shapeWorksheet.Name);
}
}
}
```
### See Also
* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
