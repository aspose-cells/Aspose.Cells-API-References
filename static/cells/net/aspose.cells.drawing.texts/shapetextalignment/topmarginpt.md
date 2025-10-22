##ShapeTextAlignment.TopMarginPt
ShapeTextAlignment property. Returns the top margin in unit of Points
## ShapeTextAlignment.TopMarginPt property
Returns the top margin in unit of Points
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
public class ShapeTextAlignmentPropertyTopMarginPtDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
shape.Text = "Sample Text";
shape.TextBody.TextAlignment.TopMarginPt = 2.0d;
workbook.Save("ShapeTextAlignmentTopMarginPtDemo.xlsx");
}
}
}
```
### See Also
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
