##PageSetup.Copy
PageSetup method. Copies the setting of the page setup
## PageSetup.Copy method
Copies the setting of the page setup.
```csharp
public void Copy(PageSetup source, CopyOptions copyOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| source | PageSetup | The source. |
| copyOptions | CopyOptions | The copy options. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupMethodCopyWithPageSetupCopyOptionsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets.Add();
// Set PageSetup properties for the first worksheet
workbook.Worksheets[0].PageSetup.PaperSize = PaperSizeType.PaperA3;
// Copy PageSetup from first worksheet to second worksheet with CopyOptions
workbook.Worksheets[1].PageSetup.Copy(workbook.Worksheets[0].PageSetup, new CopyOptions());
Console.WriteLine("Paper size of second worksheet: " + workbook.Worksheets[1].PageSetup.PaperSize);
}
}
}
```
### See Also
* class [CopyOptions](../../copyoptions/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
