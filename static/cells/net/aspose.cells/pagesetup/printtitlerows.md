##PageSetup.PrintTitleRows
PageSetup property. Represents the rows that contain the cells to be repeated at the top of each page
## PageSetup.PrintTitleRows property
Represents the rows that contain the cells to be repeated at the top of each page.
```csharp
public string PrintTitleRows { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPrintTitleRowsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set some sample data
worksheet.Cells["A1"].PutValue("Header");
for (int i = 2; i <= 10; i++)
{
worksheet.Cells["A" + i].PutValue("Data " + (i-1));
}
// Access page setup
PageSetup pageSetup = worksheet.PageSetup;
// Set print title rows (first row will repeat on each printed page)
pageSetup.PrintTitleRows = "$1:$1";
// Save the workbook
workbook.Save("PrintTitleRowsDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
