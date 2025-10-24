##Class PageStartSavingArgs
Aspose.Cells.Rendering.PageStartSavingArgs class. Info for a page starts saving process
## PageStartSavingArgs class
Info for a page starts saving process.
```csharp
public class PageStartSavingArgs : PageSavingArgs
```
## Properties
| Name | Description |
| --- | --- |
| [IsToOutput](../../aspose.cells.rendering/pagestartsavingargs/istooutput/) { get; set; } | Gets or sets a value indicating whether the page should be output. The default value is true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Total page count.(Inherited from [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Current page index, zero based.(Inherited from [`PageSavingArgs`](../pagesavingargs/).) |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class RenderingClassPageStartSavingArgsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue("Hello World");
PdfSaveOptions options = new PdfSaveOptions();
options.PageSavingCallback = new CustomPageSavingCallback();
workbook.Save("output.pdf", options);
}
}
public class CustomPageSavingCallback : IPageSavingCallback
{
public void PageStartSaving(PageStartSavingArgs args)
{
Console.WriteLine($"Starting to save page {args.PageIndex}");
}
public void PageEndSaving(PageEndSavingArgs args)
{
// Optional implementation
}
}
}
```
### See Also
* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
