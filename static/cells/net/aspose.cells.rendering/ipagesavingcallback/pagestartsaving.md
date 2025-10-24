##IPageSavingCallback.PageStartSaving
IPageSavingCallback method. Control/Indicate a page starts to be output
## IPageSavingCallback.PageStartSaving method
Control/Indicate a page starts to be output.
```csharp
public void PageStartSaving(PageStartSavingArgs args)
```
| Parameter | Type | Description |
| --- | --- | --- |
| args | PageStartSavingArgs | Info for a page starts saving process. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class IPageSavingCallbackMethodPageStartSavingWithPageStartSavingArgsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample content to create multiple pages
for (int i = 0; i < 150; i++)
worksheet.Cells[$"A{i + 1}"].Value = $"Data row {i + 1}";
PdfSaveOptions saveOptions = new PdfSaveOptions();
PageSavingCallback callback = new PageSavingCallback();
saveOptions.PageSavingCallback = callback;
try
{
workbook.Save("PageStartSavingOutput.pdf", saveOptions);
Console.WriteLine($"Processed pages: {callback.ProcessedPages}");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
public class PageSavingCallback : IPageSavingCallback
{
public int ProcessedPages { get; private set; }
public void PageStartSaving(PageStartSavingArgs args)
{
if (args.PageIndex % 3 == 0) // Skip every 3rd page (0-based)
args.IsToOutput = false;
else
ProcessedPages++;
Console.WriteLine(args.IsToOutput
? $"Saving page {args.PageIndex + 1}"
: $"Skipping page {args.PageIndex + 1}");
}
public void PageEndSaving(PageEndSavingArgs args)
{
// Optional page end handling
}
}
}
```
### See Also
* class [PageStartSavingArgs](../../pagestartsavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
