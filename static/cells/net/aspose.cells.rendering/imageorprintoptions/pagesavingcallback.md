##ImageOrPrintOptions.PageSavingCallback
ImageOrPrintOptions property. Control/Indicate progress of page saving process
## ImageOrPrintOptions.PageSavingCallback property
Control/Indicate progress of page saving process.
```csharp
public IPageSavingCallback PageSavingCallback { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;
using System;
public class ImageOrPrintOptionsPropertyPageSavingCallbackDemo
{
public static void Run()
{
// Create a new workbook and populate data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data spanning multiple pages
worksheet.Cells["A1"].PutValue("PageSavingCallback Demonstration");
for (int i = 1; i <= 50; i++)
{
worksheet.Cells[$"A{i + 1}"].PutValue($"Data Row {i}");
}
// Configure page setup to generate multiple pages
PageSetup pageSetup = worksheet.PageSetup;
pageSetup.PaperSize = PaperSizeType.PaperA4;
pageSetup.Orientation = PageOrientationType.Portrait;
pageSetup.FitToPagesWide = 1;
pageSetup.FitToPagesTall = 0;
// Initialize ImageOrPrintOptions
ImageOrPrintOptions options = new ImageOrPrintOptions
{
ImageType = ImageType.Tiff,
TiffCompression = TiffCompression.CompressionCCITT4
};
// Display initial callback state
Console.WriteLine($"Initial PageSavingCallback: {options.PageSavingCallback}");
// Set custom page saving callback
options.PageSavingCallback = new CustomPageSavingCallback();
// Render worksheet to multi-page TIFF
SheetRender renderer = new SheetRender(worksheet, options);
renderer.ToTiff("output_with_callback.tiff");
// Save workbook for reference
workbook.Save("PageSavingCallbackDemo.xlsx");
}
private class CustomPageSavingCallback : IPageSavingCallback
{
public void PageStartSaving(PageStartSavingArgs args)
{
Console.WriteLine($"Processing page {args.PageIndex}");
// Skip first page (0-based index)
if (args.PageIndex == 0)
{
args.IsToOutput = false;
Console.WriteLine("Skipping first page");
}
}
public void PageEndSaving(PageEndSavingArgs args)
{
Console.WriteLine($"Completed processing page {args.PageIndex}");
}
}
}
}
```
### See Also
* interface [IPageSavingCallback](../../ipagesavingcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
