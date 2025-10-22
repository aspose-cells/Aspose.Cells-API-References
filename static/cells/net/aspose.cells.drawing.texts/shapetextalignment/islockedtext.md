##ShapeTextAlignment.IsLockedText
ShapeTextAlignment property. Indicates whether the shape is locked when worksheet is protected
## ShapeTextAlignment.IsLockedText property
Indicates whether the shape is locked when worksheet is protected.
```csharp
public bool IsLockedText { get; set; }
```
### Remarks
Only works when worksheet is protected.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyIsLockedTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
textBox.Text = "Sample Text";
// Access the text alignment properties
Aspose.Cells.Drawing.Texts.ShapeTextAlignment textAlignment = textBox.TextBody.TextAlignment;
// Set and demonstrate IsLockedText property
textAlignment.IsLockedText = true;
Console.WriteLine("Text locked status: " + textAlignment.IsLockedText);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
