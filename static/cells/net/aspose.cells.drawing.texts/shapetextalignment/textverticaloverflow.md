##ShapeTextAlignment.TextVerticalOverflow
ShapeTextAlignment property. Gets and sets the text vertical overflow type of the text box
## ShapeTextAlignment.TextVerticalOverflow property
Gets and sets the text vertical overflow type of the text box.
```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyTextVerticalOverflowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
// Set text that might overflow vertically
shape.Text = "This is a long text that might overflow vertically if not clipped properly";
// Get text alignment and set vertical overflow to Clip
ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
// Save the workbook
workbook.Save("TextVerticalOverflowDemo.xlsx");
}
}
}
```
### See Also
* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
