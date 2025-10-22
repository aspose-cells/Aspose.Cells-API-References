##PageSavingArgs.PageCount
PageSavingArgs property. Total page count
## PageSavingArgs.PageCount property
Total page count.
```csharp
public int PageCount { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class PageSavingArgsPropertyPageCountDemo
{
public static void Run()
{
// Create a new workbook and add test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add dense content to create multiple pages
for (int i = 0; i < 500; i++)
{
worksheet.Cells[i, 0].Value = "Row " + (i + 1);
}
// Set page setup to control pagination
worksheet.PageSetup.PrintArea = "A1:A50";
worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;
// Create PDF save options with page saving callback
PdfSaveOptions options = new PdfSaveOptions();
options.PageSavingCallback = new PageSavingCallback();
// Save to PDF to trigger pagination
workbook.Save("PageSavingDemo.pdf", options);
}
private class PageSavingCallback : IPageSavingCallback
{
public void PageStartSaving(PageStartSavingArgs args)
{
// Access PageCount from the event arguments
Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
}
public void PageEndSaving(PageEndSavingArgs args)
{
// No implementation needed
}
}
}
}
```
### See Also
* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
