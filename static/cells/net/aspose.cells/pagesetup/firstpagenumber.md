##PageSetup.FirstPageNumber
PageSetup property. Represents the first page number that will be used when this sheet is printed
## PageSetup.FirstPageNumber property
Represents the first page number that will be used when this sheet is printed.
```csharp
public int FirstPageNumber { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyFirstPageNumberDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set page setup properties
worksheet.PageSetup.IsAutoFirstPageNumber = false;
worksheet.PageSetup.FirstPageNumber = 3;
// Print the results
Console.WriteLine("IsAutoFirstPageNumber: " + worksheet.PageSetup.IsAutoFirstPageNumber);
Console.WriteLine("FirstPageNumber: " + worksheet.PageSetup.FirstPageNumber);
// Save the workbook
workbook.Save("PageSetupFirstPageNumberDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
