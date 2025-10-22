##PageSetup.IsHFDiffFirst
PageSetup property. True means that the header/footer of the first page is different with other pages
## PageSetup.IsHFDiffFirst property
True means that the header/footer of the first page is different with other pages.
```csharp
public bool IsHFDiffFirst { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyIsHFDiffFirstDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access PageSetup
PageSetup pageSetup = worksheet.PageSetup;
// Set different headers/footers for first page
pageSetup.IsHFDiffFirst = true;
// Set headers/footers
pageSetup.SetFirstPageHeader(0, "First Page Header");
pageSetup.SetHeader(0, "Standard Header");
// Save the workbook
workbook.Save("PageSetup_IsHFDiffFirst_Example.xlsx");
// Reload the workbook to verify settings
Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffFirst_Example.xlsx");
PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
// Output verification
Console.WriteLine("IsHFDiffFirst: " + loadedPageSetup.IsHFDiffFirst);
Console.WriteLine("First Page Header: " + loadedPageSetup.GetFirstPageHeader(0));
Console.WriteLine("Standard Header: " + loadedPageSetup.GetHeader(0));
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
