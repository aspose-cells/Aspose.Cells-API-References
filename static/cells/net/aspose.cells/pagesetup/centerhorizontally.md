##PageSetup.CenterHorizontally
PageSetup property. Represent if the sheet is printed centered horizontally
## PageSetup.CenterHorizontally property
Represent if the sheet is printed centered horizontally.
```csharp
public bool CenterHorizontally { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyCenterHorizontallyDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
worksheet.Cells["A1"].PutValue("Sample Data");
for (int i = 1; i <= 5; i++)
{
worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
worksheet.Cells["B" + (i + 1)].PutValue(i * 100);
}
PageSetup pageSetup = worksheet.PageSetup;
// Demonstrate CenterHorizontally property
pageSetup.CenterHorizontally = true;
pageSetup.PrintArea = "A1:B6";
workbook.Save("CenterHorizontallyDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
