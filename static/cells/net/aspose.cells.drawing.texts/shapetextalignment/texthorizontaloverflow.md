##ShapeTextAlignment.TextHorizontalOverflow
ShapeTextAlignment property. Gets and sets the text horizontal overflow type of the text box
## ShapeTextAlignment.TextHorizontalOverflow property
Gets and sets the text horizontal overflow type of the text box.
```csharp
public TextOverflowType TextHorizontalOverflow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyTextHorizontalOverflowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape
TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 50);
textBox.Text = "This is a long text that demonstrates horizontal overflow behavior";
// Set horizontal overflow to Clip
textBox.TextBody.TextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
// Save the workbook
workbook.Save("TextHorizontalOverflowDemo.xlsx");
}
}
}
```
### See Also
* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
