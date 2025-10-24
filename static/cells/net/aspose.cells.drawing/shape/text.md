##Shape.Text
Shape property. Gets and sets the text of this shape
## Shape.Text property
Gets and sets the text of this shape.
```csharp
public string Text { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with correct parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
// Set text if null
if (shape.Text == null)
{
shape.Text = "This is a test.";
}
// Modify the text
shape.Text = "Updated text demo";
// Save the workbook
workbook.Save("ShapeTextDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
