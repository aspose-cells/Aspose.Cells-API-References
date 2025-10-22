##PaginatedSaveOptions.PageSavingCallback
PaginatedSaveOptions property. Control/Indicate progress of page saving process
## PaginatedSaveOptions.PageSavingCallback property
Control/Indicate progress of page saving process.
```csharp
public IPageSavingCallback PageSavingCallback { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PaginatedSaveOptionsPropertyPageSavingCallbackDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Page 1 Content");
worksheet.Cells["A2"].PutValue("This demonstrates PageSavingCallback");
// Create save options with page saving callback
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSavingCallback = new CustomPageSavingCallback();
// Save with callback
workbook.Save("PageSavingCallbackDemo.pdf", saveOptions);
}
}
public class CustomPageSavingCallback : IPageSavingCallback
{
public void PageStartSaving(PageStartSavingArgs args)
{
Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
}
public void PageEndSaving(PageEndSavingArgs args)
{
Console.WriteLine($"Finished saving page {args.PageIndex + 1}");
if (args.HasMorePages)
{
Console.WriteLine("More pages to follow...");
}
}
}
}
```
### See Also
* interface [IPageSavingCallback](../../../aspose.cells.rendering/ipagesavingcallback/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
