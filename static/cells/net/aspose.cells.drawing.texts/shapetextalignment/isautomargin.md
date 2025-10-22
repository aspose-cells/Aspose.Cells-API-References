##ShapeTextAlignment.IsAutoMargin
ShapeTextAlignment property. Indicates whether the margin of the text frame is automatic
## ShapeTextAlignment.IsAutoMargin property
Indicates whether the margin of the text frame is automatic.
```csharp
public bool IsAutoMargin { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class ShapeTextAlignmentPropertyIsAutoMarginDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
// Access text alignment and set IsAutoMargin
shape.TextBody.TextAlignment.IsAutoMargin = true;
// Set some text to demonstrate
shape.Text = "Sample text with auto margins";
// Save the workbook
workbook.Save("ShapeTextAlignmentIsAutoMarginDemo.xlsx");
}
}
}
```
### See Also
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
