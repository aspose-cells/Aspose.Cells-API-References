##PageSetup.PrintGridlines
PageSetup property. Represents if cell gridlines are printed on the page
## PageSetup.PrintGridlines property
Represents if cell gridlines are printed on the page.
```csharp
public bool PrintGridlines { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPrintGridlinesDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Put sample data in cell
worksheet.Cells["A1"].PutValue("PrintGridlines Property Demo");
worksheet.Cells["A3"].PutValue("Gridlines will ");
worksheet.Cells["B3"].PutValue(worksheet.PageSetup.PrintGridlines ? "appear" : "not appear");
worksheet.Cells["A4"].PutValue("when printing this sheet.");
// Toggle PrintGridlines property
worksheet.PageSetup.PrintGridlines = true;
// Save the workbook
workbook.Save("PrintGridlinesDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
