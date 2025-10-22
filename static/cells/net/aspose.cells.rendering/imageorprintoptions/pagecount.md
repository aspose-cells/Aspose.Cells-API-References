##ImageOrPrintOptions.PageCount
ImageOrPrintOptions property. Gets or sets the number of pages to save
## ImageOrPrintOptions.PageCount property
Gets or sets the number of pages to save.
```csharp
public int PageCount { get; set; }
```
### Remarks
Default is System.Int32.MaxValue which means all pages will be rendered.
### Examples
```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyPageCountDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Page 1 Data");
worksheet.Cells["A2"].PutValue("Sample Content");
worksheet.Cells["A3"].PutValue("Demo for PageCount");
// Set print area and page setup
worksheet.PageSetup.PrintArea = "A1:A3";
worksheet.PageSetup.LeftMargin = 0;
worksheet.PageSetup.RightMargin = 0;
worksheet.PageSetup.TopMargin = 0;
worksheet.PageSetup.BottomMargin = 0;
// Create image or print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.OnePagePerSheet = true;
options.ImageType = Aspose.Cells.Drawing.ImageType.Png; // Fully qualified namespace AsposeCellsExamples = 1; // Demonstrating PageCount property
options.OnlyArea = true;
// Render the worksheet to image
SheetRender renderer = new SheetRender(worksheet, options);
using (MemoryStream stream = new MemoryStream())
{
renderer.ToImage(0, stream);
// Save the image to file
string outputPath = "output.png";
File.WriteAllBytes(outputPath, stream.ToArray());
Console.WriteLine($"Output saved to: {outputPath}");
}
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
