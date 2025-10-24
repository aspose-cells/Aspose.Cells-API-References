##TextBoxOptions.LeftMarginPt
TextBoxOptions property. Gets and sets the left margin in unit of Points
## TextBoxOptions.LeftMarginPt property
Gets and sets the left margin in unit of Points.
```csharp
public double LeftMarginPt { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextBoxOptionsPropertyLeftMarginPtDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 400);
textBox.TextBoxOptions.LeftMarginPt = 0.2d;
Console.WriteLine("Left margin set to: " + textBox.TextBoxOptions.LeftMarginPt + " points");
}
}
}
```
### See Also
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
