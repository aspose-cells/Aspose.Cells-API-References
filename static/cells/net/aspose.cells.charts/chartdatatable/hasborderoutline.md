##ChartDataTable.HasBorderOutline
ChartDataTable property. True if the chart data table has outline borders
## ChartDataTable.HasBorderOutline property
True if the chart data table has outline borders
```csharp
[Obsolete("Use ChartDataTable.HasOutlineBorder property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBorderOutline { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasOutlineBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartDataTablePropertyHasBorderOutlineDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["B2"].PutValue(50);
worksheet.Cells["B3"].PutValue(30);
// Add chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Enable and configure data table
chart.ShowDataTable = true;
ChartDataTable chartTable = chart.ChartDataTable;
// Demonstrate HasBorderOutline property
chartTable.HasBorderOutline = true;
chartTable.HasBorderHorizontal = true;
chartTable.HasBorderVertical = true;
chartTable.Font.Color = Color.Blue;
workbook.Save("ChartDataTableWithBorderOutline.xlsx");
}
}
}
```
### See Also
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
