##Enum PlacementType
Aspose.Cells.Drawing.PlacementType enum. Represents the way the drawing object is attached to the cells below it
## PlacementType enumeration
Represents the way the drawing object is attached to the cells below it.
```csharp
public enum PlacementType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| FreeFloating | `0` | Don't move or size with cells. |
| Move | `1` | Move but don't size with cells. |
| MoveAndSize | `2` | Move and size with cells. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
public class PlacementTypeDemo
{
public static void PlacementTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set the chart data range
chart.SetChartDataRange("A1:B4", true);
// Set the placement type of the chart
chart.Placement = PlacementType.MoveAndSize;
// Output the placement type
Console.WriteLine("Chart Placement Type: " + chart.Placement);
// Save the workbook
workbook.Save("PlacementTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
