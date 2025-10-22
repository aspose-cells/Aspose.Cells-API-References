##ChartDataTable.HasBorderVertical
ChartDataTable property. True if the chart data table has vertical cell borders
## ChartDataTable.HasBorderVertical property
True if the chart data table has vertical cell borders
```csharp
[Obsolete("Use ChartDataTable.HasVerticalBorder property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBorderVertical { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasVerticalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartDataTablePropertyHasBorderVerticalDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
chart.ShowDataTable = true;
ChartDataTable chartTable = chart.ChartDataTable;
chartTable.HasBorderVertical = true;
chartTable.HasBorderHorizontal = true;
workbook.Save("ChartDataTable_HasBorderVertical.xlsx");
}
}
}
```
### See Also
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
