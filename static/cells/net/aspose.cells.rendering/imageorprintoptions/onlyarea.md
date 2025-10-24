##ImageOrPrintOptions.OnlyArea
ImageOrPrintOptions property. If this property is true  one Area will be output and no scale will take effect
## ImageOrPrintOptions.OnlyArea property
If this property is true , one Area will be output, and no scale will take effect.
```csharp
public bool OnlyArea { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyOnlyAreaDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Set image options with OnlyArea property
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.OnePagePerSheet = true;
options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
options.OnlyArea = true; // Only render the used area
// Render worksheet to image
SheetRender sr = new SheetRender(worksheet, options);
using (MemoryStream ms = new MemoryStream())
{
sr.ToImage(0, ms);
Console.WriteLine("Worksheet rendered to image with OnlyArea=true");
}
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
