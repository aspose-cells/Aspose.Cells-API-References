##SaveOptions.UpdateSmartArt
SaveOptions property. Indicates whether updating smart art setting. The default value is false
## SaveOptions.UpdateSmartArt property
Indicates whether updating smart art setting. The default value is false.
```csharp
public bool UpdateSmartArt { get; set; }
```
### Remarks
Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class SaveOptionsPropertyUpdateSmartArtDemo
{
public static void Run()
{
// Load the source workbook
Workbook workbook = new Workbook("example.xlsx");
// Modify shapes and SmartArt
foreach (Worksheet worksheet in workbook.Worksheets)
{
foreach (Shape shape in worksheet.Shapes)
{
shape.AlternativeText = "ReplacedAlternativeText";
if (shape.IsSmartArt)
{
foreach (Shape smartArtShape in shape.GetResultOfSmartArt().GetGroupedShapes())
{
smartArtShape.Text = "ReplacedText";
}
}
}
}
// Save with UpdateSmartArt enabled
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
saveOptions.UpdateSmartArt = true;
workbook.Save("output.xlsx", saveOptions);
// Verify the changes
Workbook savedWorkbook = new Workbook("output.xlsx");
foreach (Worksheet worksheet in savedWorkbook.Worksheets)
{
foreach (Shape shape in worksheet.Shapes)
{
Console.WriteLine($"Shape Alt Text: {shape.AlternativeText}");
if (shape.IsSmartArt)
{
foreach (Shape smartArtShape in shape.GetResultOfSmartArt().GetGroupedShapes())
{
Console.WriteLine($"SmartArt Text: {smartArtShape.Text}");
}
}
}
}
}
}
}
```
### See Also
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
