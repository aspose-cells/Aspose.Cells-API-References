##PageEndSavingArgs.HasMorePages
PageEndSavingArgs property. Gets or sets a value indicating whether having more pages to be output. The default value is true
## PageEndSavingArgs.HasMorePages property
Gets or sets a value indicating whether having more pages to be output. The default value is true.
```csharp
public bool HasMorePages { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class PageEndSavingArgsPropertyHasMorePagesDemo
{
public static void Run()
{
// Create a workbook with data spanning multiple pages
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
for (int i = 0; i < 500; i++)
{
worksheet.Cells[i, 0].Value = $"Row {i + 1}";
}
// Create PDF save options with custom page handling
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSavingCallback = new PageControlCallback();
// Save workbook with page limitation
workbook.Save("PropertyHasMorePagesDemo.pdf", saveOptions);
}
}
internal class PageControlCallback : IPageSavingCallback
{
private int pageCount = 0;
public void PageStartSaving(PageStartSavingArgs args)
{
// Not used in this demonstration
}
public void PageEndSaving(PageEndSavingArgs args)
{
// Read current property value
Console.WriteLine($"Page {pageCount} - Initial HasMorePages: {args.HasMorePages}");
// Modify property after first page
if (pageCount == 0)
{
args.HasMorePages = false;
Console.WriteLine($"Page {pageCount} - Updated HasMorePages: {args.HasMorePages}");
}
pageCount++;
}
}
}
```
### See Also
* class [PageEndSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
