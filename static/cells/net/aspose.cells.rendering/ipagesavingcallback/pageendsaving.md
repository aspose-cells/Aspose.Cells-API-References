##IPageSavingCallback.PageEndSaving
IPageSavingCallback method. Control/Indicate a page ends to be output
## IPageSavingCallback.PageEndSaving method
Control/Indicate a page ends to be output.
```csharp
public void PageEndSaving(PageEndSavingArgs args)
```
| Parameter | Type | Description |
| --- | --- | --- |
| args | PageEndSavingArgs | Info for a page ends saving process. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class IPageSavingCallbackMethodPageEndSavingWithPageEndSavingArgsDemo
{
public static void Run()
{
// Create a new workbook and populate data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create multiple pages when rendered
for (int i = 0; i < 500; i++)
{
worksheet.Cells[$"A{i+1}"].Value = $"Row {i+1} - Demonstration data for page splitting";
}
// Create PDF save options with custom page saving callback
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSavingCallback = new PageEndSavingCallback();
try
{
// Save workbook with callback implementation
workbook.Save("PageEndSavingDemo.pdf", saveOptions);
Console.WriteLine("Document saved successfully with page end tracking.");
}
catch (Exception ex)
{
Console.WriteLine($"Error during document save: {ex.Message}");
}
}
private class PageEndSavingCallback : IPageSavingCallback
{
public void PageEndSaving(PageEndSavingArgs args)
{
// Display page saving completion information
Console.WriteLine($"Finished processing page {args.PageIndex + 1}");
// You could add file operations or other post-processing here
// args.HasMorePages shows if more pages will be processed
}
public void PageStartSaving(PageStartSavingArgs args)
{
// Required interface implementation
}
}
}
}
```
### See Also
* class [PageEndSavingArgs](../../pageendsavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
