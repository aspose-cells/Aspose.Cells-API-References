##PageSetup.PrintTitleColumns
PageSetup property. Represents the columns that contain the cells to be repeated on the left side of each page
## PageSetup.PrintTitleColumns property
Represents the columns that contain the cells to be repeated on the left side of each page.
```csharp
public string PrintTitleColumns { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPrintTitleColumnsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access page setup
PageSetup pageSetup = worksheet.PageSetup;
// Set print title columns to repeat column A on each printed page
pageSetup.PrintTitleColumns = "$A:$A";
// Add some data to column A to demonstrate the effect
for (int i = 0; i < 50; i++)
{
worksheet.Cells[$"A{i + 1}"].PutValue($"Title Column - Row {i + 1}");
}
// Save the workbook
workbook.Save("PrintTitleColumnsDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
