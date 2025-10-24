##Shape.UpperLeftColumn
Shape property. Represents upper left corner column index
## Shape.UpperLeftColumn property
Represents upper left corner column index.
```csharp
public int UpperLeftColumn { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyUpperLeftColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 100);
// Set and demonstrate UpperLeftColumn property
shape.UpperLeftColumn = 3;
Console.WriteLine("Shape's initial UpperLeftColumn: " + shape.UpperLeftColumn);
// Modify the UpperLeftColumn
if (shape.UpperLeftColumn == 3)
{
shape.UpperLeftColumn = 1;
Console.WriteLine("Shape's modified UpperLeftColumn: " + shape.UpperLeftColumn);
}
// Save the workbook
workbook.Save("ShapeUpperLeftColumnDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
