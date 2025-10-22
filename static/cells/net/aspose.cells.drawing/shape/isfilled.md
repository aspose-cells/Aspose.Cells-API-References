##Shape.IsFilled
Shape property. Indicates whether the fill format is visible
## Shape.IsFilled property
Indicates whether the fill format is visible.
```csharp
public bool IsFilled { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsFilledDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);
// Check and modify IsFilled property
if (shape.IsFilled == false)
{
shape.IsFilled = true;
shape.FillFormat.ForeColor = System.Drawing.Color.Red;
}
// Save the workbook
workbook.Save("ShapeIsFilledDemo_out.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
