##PageSetup.GetFirstPageHeader
PageSetup method. Gets a script formatting the first page header of an Excel file
## PageSetup.GetFirstPageHeader method
Gets a script formatting the first page header of an Excel file.
```csharp
public string GetFirstPageHeader(int section)
```
| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupMethodGetFirstPageHeaderWithInt32Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access PageSetup
PageSetup pageSetup = worksheet.PageSetup;
// Enable different first page header/footer
pageSetup.IsHFDiffFirst = true;
// Set first page header sections
pageSetup.SetFirstPageHeader(0, "&LFirst Page Left Header");
pageSetup.SetFirstPageHeader(1, "&CFirst Page Center Header");
pageSetup.SetFirstPageHeader(2, "&RFirst Page Right Header");
// Get and display first page header sections
Console.WriteLine("First Page Header Sections:");
Console.WriteLine("Left: " + pageSetup.GetFirstPageHeader(0));
Console.WriteLine("Center: " + pageSetup.GetFirstPageHeader(1));
Console.WriteLine("Right: " + pageSetup.GetFirstPageHeader(2));
// Save the workbook
workbook.Save("PageSetupFirstPageHeaderDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
