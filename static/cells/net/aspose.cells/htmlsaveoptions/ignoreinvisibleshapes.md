##HtmlSaveOptions.IgnoreInvisibleShapes
HtmlSaveOptions property. Indicate whether exporting those not visible shapes
## HtmlSaveOptions.IgnoreInvisibleShapes property
Indicate whether exporting those not visible shapes
```csharp
public bool IgnoreInvisibleShapes { get; set; }
```
### Remarks
The default values is false.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyIgnoreInvisibleShapesDemo
{
public static void Run()
{
// Create a workbook with a sample worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add visible and invisible shapes
Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 50, 50);
shape1.IsHidden = false;
Shape shape2 = worksheet.Shapes.AddRectangle(1, 0, 100, 100, 50, 50);
shape2.IsHidden = true;
// Save with IgnoreInvisibleShapes = true (default)
HtmlSaveOptions saveOptions1 = new HtmlSaveOptions();
saveOptions1.IgnoreInvisibleShapes = true;
workbook.Save("output_ignore_invisible.html", saveOptions1);
// Save with IgnoreInvisibleShapes = false
HtmlSaveOptions saveOptions2 = new HtmlSaveOptions();
saveOptions2.IgnoreInvisibleShapes = false;
workbook.Save("output_include_invisible.html", saveOptions2);
Console.WriteLine("HTML files saved with different IgnoreInvisibleShapes settings.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
