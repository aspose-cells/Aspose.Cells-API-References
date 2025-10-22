##Worksheet.Shapes
Worksheet property. Returns all drawing shapes in this worksheet
## Worksheet.Shapes property
Returns all drawing shapes in this worksheet.
```csharp
public ShapeCollection Shapes { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class WorksheetPropertyShapesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Add some shapes to the worksheet
sheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
sheet.Shapes.AddLine(2, 0, 100, 100, 100, 1);
// Modify shape properties
for (int i = 0; i < sheet.Shapes.Count; i++)
{
Aspose.Cells.Drawing.Shape shape = sheet.Shapes[i];
Console.WriteLine($"Shape {i}: Type={shape.Type}, Name={shape.Name}");
// Update properties for the first shape
if (i == 0)
{
shape.Name = "MyRectangle";
shape.FillFormat.ForeColor = System.Drawing.Color.Red;
}
}
// Save the workbook
workbook.Save("ShapesDemo.xlsx");
}
}
}
```
### See Also
* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
