##TextBoxOptions.AllowTextToOverflow
TextBoxOptions property. Whether allow text to overflow shape
## TextBoxOptions.AllowTextToOverflow property
Whether allow text to overflow shape.
```csharp
public bool AllowTextToOverflow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextBoxOptionsPropertyAllowTextToOverflowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
// Set text that might overflow
textBox.Text = "This is a long text that might overflow the text box boundaries if AllowTextToOverflow is false";
// Enable text overflow
textBox.TextBoxOptions.AllowTextToOverflow = true;
// Save the workbook
workbook.Save("TextBoxAllowTextToOverflowDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
