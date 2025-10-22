##Series.UpBars
Series property. Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts
## Series.UpBars property
Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts.
```csharp
public DropBars UpBars { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SeriesPropertyUpBarsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data for line chart with up/down bars
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Enable and customize up bars
chart.NSeries[0].HasUpDownBars = true;
DropBars upBars = chart.NSeries[0].UpBars;
upBars.Area.ForegroundColor = Color.LightGreen;
upBars.Border.Color = Color.Green;
workbook.Save("UpBarsExample.xlsx");
}
}
}
```
### See Also
* class [DropBars](../../dropbars/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
