##ShapeTextAlignment.BottomMarginPt
ShapeTextAlignment property. Returns the bottom margin in unit of Points
## ShapeTextAlignment.BottomMarginPt property
Returns the bottom margin in unit of Points
```csharp
public double BottomMarginPt { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyBottomMarginPtDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
shape.Text = "Sample Text";
shape.TextBody.TextAlignment.BottomMarginPt = 2.0d;
Console.WriteLine("Bottom margin set to: " + shape.TextBody.TextAlignment.BottomMarginPt + " points");
}
}
}
```
### See Also
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
