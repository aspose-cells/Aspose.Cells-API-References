##PageSetup.IsHFScaleWithDoc
PageSetup property. Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007
## PageSetup.IsHFScaleWithDoc property
Indicates whether header and footer are scaled with document scaling. Only applies for Excel 2007.
```csharp
public bool IsHFScaleWithDoc { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyIsHFScaleWithDocDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access PageSetup
PageSetup pageSetup = worksheet.PageSetup;
// Set basic page setup
pageSetup.Orientation = PageOrientationType.Landscape;
pageSetup.PaperSize = PaperSizeType.PaperA4;
// Demonstrate IsHFScaleWithDoc property
pageSetup.IsHFScaleWithDoc = true;
Console.WriteLine("Header/Footer scaling with document is set to: " + pageSetup.IsHFScaleWithDoc);
// Save the workbook
workbook.Save("PageSetup_IsHFScaleWithDoc_Demo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
