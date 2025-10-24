##ShapeTextAlignment.TextVerticalType
ShapeTextAlignment property. Gets and sets the text direction
## ShapeTextAlignment.TextVerticalType property
Gets and sets the text direction.
```csharp
public TextVerticalType TextVerticalType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyTextVerticalTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape with correct parameters
Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
shape.Text = "Sample Text";
// Get the text alignment and set vertical text type
ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
textAlignment.TextVerticalType = TextVerticalType.Horizontal;
// Save the workbook
workbook.Save("TextVerticalTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [TextVerticalType](../../textverticaltype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
