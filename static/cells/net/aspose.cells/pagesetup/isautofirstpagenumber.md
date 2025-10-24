##PageSetup.IsAutoFirstPageNumber
PageSetup property. Indicates whether the first the page number is automatically assigned
## PageSetup.IsAutoFirstPageNumber property
Indicates whether the first the page number is automatically assigned.
```csharp
public bool IsAutoFirstPageNumber { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyIsAutoFirstPageNumberDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set page setup properties
worksheet.PageSetup.IsAutoFirstPageNumber = true;
Console.WriteLine("Auto First Page Number (Worksheet 1): " + worksheet.PageSetup.IsAutoFirstPageNumber);
// Add a second worksheet
worksheet = workbook.Worksheets.Add("Sheet2");
worksheet.PageSetup.IsAutoFirstPageNumber = false;
worksheet.PageSetup.FirstPageNumber = 3;
Console.WriteLine("Auto First Page Number (Worksheet 2): " + worksheet.PageSetup.IsAutoFirstPageNumber);
Console.WriteLine("First Page Number (Worksheet 2): " + worksheet.PageSetup.FirstPageNumber);
// Save the workbook
workbook.Save("PageSetup_IsAutoFirstPageNumber_Example.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
