##PageSetup.IsPercentScale
PageSetup property. If this property is False the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled
## PageSetup.IsPercentScale property
If this property is False, the FitToPagesWide and FitToPagesTall properties control how the worksheet is scaled.
```csharp
public bool IsPercentScale { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyIsPercentScaleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access PageSetup and set scaling to 80% (percent scale)
PageSetup pageSetup = worksheet.PageSetup;
pageSetup.Zoom = 80;
pageSetup.IsPercentScale = true;
// Output the settings to demonstrate IsPercentScale
Console.WriteLine("Zoom: " + pageSetup.Zoom);
Console.WriteLine("IsPercentScale: " + pageSetup.IsPercentScale);
// Save the workbook
workbook.Save("PageSetup_IsPercentScale_Output.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
