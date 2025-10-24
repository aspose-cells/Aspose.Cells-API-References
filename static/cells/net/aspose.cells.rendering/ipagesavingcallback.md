##Interface IPageSavingCallback
Aspose.Cells.Rendering.IPageSavingCallback interface. Control/Indicate progress of page saving process
## IPageSavingCallback interface
Control/Indicate progress of page saving process.
```csharp
public interface IPageSavingCallback
```
## Methods
| Name | Description |
| --- | --- |
| [PageEndSaving](../../aspose.cells.rendering/ipagesavingcallback/pageendsaving/)(PageEndSavingArgs) | Control/Indicate a page ends to be output. |
| [PageStartSaving](../../aspose.cells.rendering/ipagesavingcallback/pagestartsaving/)(PageStartSavingArgs) | Control/Indicate a page starts to be output. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class PageSavingCallbackDemo : IPageSavingCallback
{
public static void PageSavingCallbackExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["A2"].PutValue("World");
// Create save options with a page saving callback
DocxSaveOptions saveOptions = new DocxSaveOptions();
saveOptions.PageSavingCallback = new PageSavingCallbackDemo();
// Save the workbook as a DOCX file
workbook.Save("PageSavingCallbackExample.docx", saveOptions);
}
// Implement the PageStartSaving method
public void PageStartSaving(PageStartSavingArgs args)
{
Console.WriteLine($"Starting to save page {args.PageIndex}");
}
// Implement the PageEndSaving method
public void PageEndSaving(PageEndSavingArgs args)
{
Console.WriteLine($"Finished saving page {args.PageIndex}");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
