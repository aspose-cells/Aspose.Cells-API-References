##Shape.TextVerticalOverflow
Shape property. Gets and sets the text vertical overflow type of the shape which contains text
## Shape.TextVerticalOverflow property
Gets and sets the text vertical overflow type of the shape which contains text.
```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTextVerticalOverflowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
// Set text and make it overflow vertically
shape.Text = "This is a long text that will demonstrate vertical text overflow functionality in the shape.";
shape.TextVerticalOverflow = TextOverflowType.Overflow;
// Save the workbook
workbook.Save("ShapeTextVerticalOverflowDemo.xlsx");
}
}
}
```
### See Also
* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
