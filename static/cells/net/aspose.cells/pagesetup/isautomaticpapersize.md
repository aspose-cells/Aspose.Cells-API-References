##PageSetup.IsAutomaticPaperSize
PageSetup property. Indicates whether the paper size is automatic
## PageSetup.IsAutomaticPaperSize property
Indicates whether the paper size is automatic.
```csharp
public bool IsAutomaticPaperSize { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyIsAutomaticPaperSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access page setup
PageSetup pageSetup = worksheet.PageSetup;
// Get automatic paper size value
Console.WriteLine("Automatic Paper Size: " + pageSetup.IsAutomaticPaperSize);
// Create another workbook with different settings
Workbook workbook2 = new Workbook("example.xlsx");
PageSetup pageSetup2 = workbook2.Worksheets[0].PageSetup;
Console.WriteLine("Automatic Paper Size from file: " + pageSetup2.IsAutomaticPaperSize);
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
