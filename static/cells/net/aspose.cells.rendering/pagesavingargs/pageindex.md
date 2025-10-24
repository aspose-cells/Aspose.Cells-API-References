##PageSavingArgs.PageIndex
PageSavingArgs property. Current page index zero based
## PageSavingArgs.PageIndex property
Current page index, zero based.
```csharp
public int PageIndex { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PageSavingArgsPropertyPageIndexDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
}
// Create PDF save options
PdfSaveOptions options = new PdfSaveOptions();
// Set the page saving callback
options.PageSavingCallback = new PageSavingCallback();
// Save the workbook to PDF - this will trigger the callback for each page
workbook.Save("output.pdf", options);
}
}
public class PageSavingCallback : IPageSavingCallback
{
public void PageStartSaving(PageStartSavingArgs args)
{
// Demonstrate PageIndex property usage
Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
}
public void PageEndSaving(PageEndSavingArgs args)
{
// Not used in this example
}
}
}
```
### See Also
* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
