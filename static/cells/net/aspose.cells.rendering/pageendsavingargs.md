##Class PageEndSavingArgs
Aspose.Cells.Rendering.PageEndSavingArgs class. Info for a page ends saving process
## PageEndSavingArgs class
Info for a page ends saving process.
```csharp
public class PageEndSavingArgs : PageSavingArgs
```
## Properties
| Name | Description |
| --- | --- |
| [HasMorePages](../../aspose.cells.rendering/pageendsavingargs/hasmorepages/) { get; set; } | Gets or sets a value indicating whether having more pages to be output. The default value is true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Total page count.(Inherited from [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Current page index, zero based.(Inherited from [`PageSavingArgs`](../pagesavingargs/).) |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class RenderingClassPageEndSavingArgsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue("Hello World!");
// Create an instance of PdfSaveOptions
PdfSaveOptions saveOptions = new PdfSaveOptions();
// Set the PageEndSaving callback
saveOptions.PageSavingCallback = new PageEndSavingArgsTest();
// Save the workbook with the callback
workbook.Save("output.pdf", saveOptions);
}
}
public class PageEndSavingArgsTest : IPageSavingCallback
{
public void PageEndSaving(PageEndSavingArgs args)
{
Console.WriteLine($"Finished saving page {args.PageIndex}");
}
public void PageStartSaving(PageStartSavingArgs args)
{
// Implementation not needed for this demo
}
}
}
```
### See Also
* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
