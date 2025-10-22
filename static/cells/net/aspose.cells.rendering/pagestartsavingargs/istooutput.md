##PageStartSavingArgs.IsToOutput
PageStartSavingArgs property. Gets or sets a value indicating whether the page should be output. The default value is true
## PageStartSavingArgs.IsToOutput property
Gets or sets a value indicating whether the page should be output. The default value is true.
```csharp
public bool IsToOutput { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class PageStartSavingArgsPropertyIsToOutputDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate data to create multiple pages
for (int i = 0; i < 100; i++)
{
worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
// Corrected: Access row height through worksheet's Rows collection
worksheet.Cells.Rows[i].Height = 50;
}
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSavingCallback = new CustomPageSavingCallback();
workbook.Save("PageOutputDemo.pdf", saveOptions);
}
private class CustomPageSavingCallback : IPageSavingCallback
{
public void PageStartSaving(PageStartSavingArgs args)
{
// Read current value
Console.WriteLine($"Page {args.PageIndex + 1} - Initial IsToOutput: {args.IsToOutput}");
// Skip every even-numbered page (1-based numbering)
if ((args.PageIndex + 1) % 2 == 0)
{
args.IsToOutput = false;
Console.WriteLine($"Disabling output for page {args.PageIndex + 1}");
}
}
public void PageEndSaving(PageEndSavingArgs args)
{
// Implementation not required for this demonstration
}
}
}
}
```
### See Also
* class [PageStartSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
