##TextBoxOptions.RightMarginPt
TextBoxOptions property. Gets and sets the right margin in unit of Points
## TextBoxOptions.RightMarginPt property
Gets and sets the right margin in unit of Points.
```csharp
public double RightMarginPt { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextBoxOptionsPropertyRightMarginPtDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
int textBoxIndex = worksheet.TextBoxes.Add(1, 1, 200, 200);
TextBox textBox = worksheet.TextBoxes[textBoxIndex];
textBox.Text = "Sample Text";
// Set the right margin in points
textBox.TextBoxOptions.RightMarginPt = 0.2d;
// Save the workbook
workbook.Save("TextBoxRightMarginDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
