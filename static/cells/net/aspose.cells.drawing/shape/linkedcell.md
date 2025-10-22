##Shape.LinkedCell
Shape property. Gets or sets the worksheet range linked to the controls value
## Shape.LinkedCell property
Gets or sets the worksheet range linked to the control's value.
```csharp
public string LinkedCell { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyLinkedCellDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
// Set the LinkedCell property to B6
shape.LinkedCell = "$B$6";
// Change the LinkedCell to A1 if it was B6
if (shape.LinkedCell.Equals("$B$6"))
{
shape.LinkedCell = "A1";
}
// Output the current LinkedCell value
Console.WriteLine("Shape's LinkedCell: " + shape.LinkedCell);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
