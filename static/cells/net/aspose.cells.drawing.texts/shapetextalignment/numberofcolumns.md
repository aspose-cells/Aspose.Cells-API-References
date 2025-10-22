##ShapeTextAlignment.NumberOfColumns
ShapeTextAlignment property. Gets and sets the number of columns of text in the bounding rectangle
## ShapeTextAlignment.NumberOfColumns property
Gets and sets the number of columns of text in the bounding rectangle.
```csharp
public int NumberOfColumns { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyNumberOfColumnsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
// Set text for the shape
shape.Text = "This is sample text\nin multiple columns";
// Access text alignment and set number of columns
shape.TextBody.TextAlignment.NumberOfColumns = 2;
// Save the workbook
workbook.Save("output.xlsx");
// Verify the property
Console.WriteLine("Number of columns: " +
worksheet.Shapes[0].TextBody.TextAlignment.NumberOfColumns);
}
}
}
```
### See Also
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
