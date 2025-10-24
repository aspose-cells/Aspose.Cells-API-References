##TextBoxOptions.TopMarginPt
TextBoxOptions property. Gets and sets the top margin in unit of Points
## TextBoxOptions.TopMarginPt property
Gets and sets the top margin in unit of Points.
```csharp
public double TopMarginPt { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextBoxOptionsPropertyTopMarginPtDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
// Set top margin in points
textBox.TextBoxOptions.TopMarginPt = 0.2d;
// Save the workbook
workbook.Save("TextBoxTopMarginDemo.xlsx");
}
}
}
```
### See Also
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
