##PageSetup.IsHFAlignMargins
PageSetup property. Indicates whether header and footer margins are aligned with the page margins. If this property is true the left header and footer will be aligned with the left margin and the right header and footer will be aligned with the right margin. This option is enabled by default
## PageSetup.IsHFAlignMargins property
Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default.
```csharp
public bool IsHFAlignMargins { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyIsHFAlignMarginsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access the PageSetup
PageSetup pageSetup = worksheet.PageSetup;
// Set IsHFAlignMargins to true
pageSetup.IsHFAlignMargins = true;
Console.WriteLine("IsHFAlignMargins set to: " + pageSetup.IsHFAlignMargins);
// Change IsHFAlignMargins to false
pageSetup.IsHFAlignMargins = false;
Console.WriteLine("IsHFAlignMargins changed to: " + pageSetup.IsHFAlignMargins);
// Save the workbook
workbook.Save("PageSetup_IsHFAlignMargins_Example.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
