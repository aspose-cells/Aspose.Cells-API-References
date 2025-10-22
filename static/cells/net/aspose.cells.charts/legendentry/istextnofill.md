##LegendEntry.IsTextNoFill
LegendEntry property. Gets or sets no fill of the text
## LegendEntry.IsTextNoFill property
Gets or sets no fill of the text.
```csharp
public bool IsTextNoFill { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class LegendEntryPropertyIsTextNoFillDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["C1"].PutValue("Q1");
worksheet.Cells["C2"].PutValue("Q2");
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B2", true);
chart.NSeries.CategoryData = "C1:C2";
// Access legend entry and set IsTextNoFill
LegendEntry legendEntry = chart.NSeries[0].LegendEntry;
legendEntry.IsTextNoFill = true; // Text will have no fill
// Save the workbook
workbook.Save("LegendEntryIsTextNoFillDemo.xlsx");
}
}
}
```
### See Also
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
