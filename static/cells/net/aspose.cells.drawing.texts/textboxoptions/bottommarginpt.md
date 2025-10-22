##TextBoxOptions.BottomMarginPt
TextBoxOptions property. Returns the bottom margin in unit of Points
## TextBoxOptions.BottomMarginPt property
Returns the bottom margin in unit of Points
```csharp
public double BottomMarginPt { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextBoxOptionsPropertyBottomMarginPtDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
shape.TextBoxOptions.BottomMarginPt = 0.2d;
Console.WriteLine("Bottom margin set to: " + shape.TextBoxOptions.BottomMarginPt + " points");
}
}
}
```
### See Also
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
