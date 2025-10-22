##PageSetup.CenterVertically
PageSetup property. Represent if the sheet is printed centered vertically
## PageSetup.CenterVertically property
Represent if the sheet is printed centered vertically.
```csharp
public bool CenterVertically { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyCenterVerticallyDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access PageSetup and set CenterVertically
PageSetup pageSetup = worksheet.PageSetup;
pageSetup.CenterVertically = true;
// Add some sample data to visualize the effect
worksheet.Cells["A1"].PutValue("This worksheet content will be centered vertically when printed");
worksheet.Cells["A2"].PutValue("CenterVertically = true");
// Save the workbook
workbook.Save("PageSetup_CenterVertically.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
