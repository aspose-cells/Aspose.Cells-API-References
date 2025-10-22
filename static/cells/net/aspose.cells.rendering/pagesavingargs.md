##Class PageSavingArgs
Aspose.Cells.Rendering.PageSavingArgs class. Info for a page saving process
## PageSavingArgs class
Info for a page saving process.
```csharp
public class PageSavingArgs
```
## Properties
| Name | Description |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Total page count. |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Current page index, zero based. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class RenderingClassPageSavingArgsDemo
{
public static void Run()
{
// Create a new workbook with extended data for multiple pages
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate worksheet to generate multiple pages when rendered
for (int row = 0; row < 150; row++)
{
worksheet.Cells[row, 0].Value = $"Row {row + 1} data";
}
// Configure PDF save options with page saving callback
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSavingCallback = new PageSavingCallback();
// Save workbook to PDF format with pagination
workbook.Save("RenderingPageSavingDemo.pdf", pdfSaveOptions);
}
private class PageSavingCallback : IPageSavingCallback
{
public void PageStartSaving(PageStartSavingArgs args)
{
Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
if (args.PageIndex == 0)
{
Console.WriteLine("Processing cover page...");
}
}
public void PageEndSaving(PageEndSavingArgs args)
{
// Optional: Add any end-of-page processing here
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
