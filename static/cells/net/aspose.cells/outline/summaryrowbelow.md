##Outline.SummaryRowBelow
Outline property. Indicates if the summary row will be positioned below the detail rows in the outline
## Outline.SummaryRowBelow property
Indicates if the summary row will be positioned below the detail rows in the outline.
```csharp
public bool SummaryRowBelow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OutlinePropertySummaryRowBelowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and grouping
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["B1"].PutValue("Amount");
worksheet.Cells["A2"].PutValue("Product A");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("Product B");
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["A4"].PutValue("Total");
worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");
// Group rows and set summary row position
worksheet.Cells.GroupRows(1, 2, false);
Outline outline = worksheet.Outline;
outline.SummaryRowBelow = true;
workbook.Save("OutlineSummaryRowBelow.xlsx");
}
}
}
```
### See Also
* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
