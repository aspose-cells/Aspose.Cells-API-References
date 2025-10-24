##Marker.Area
Marker property. Gets the area
## Marker.Area property
Gets the `area`.
```csharp
public Area Area { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class MarkerPropertyAreaDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A3", true);
chart.NSeries[0].Marker.Area.ForegroundColor = Color.Red;
workbook.Save("MarkerPropertyAreaDemo.xlsx");
Workbook reloadedWorkbook = new Workbook("MarkerPropertyAreaDemo.xlsx");
Chart reloadedChart = reloadedWorkbook.Worksheets[0].Charts[0];
Console.WriteLine("Marker Area Color: " + reloadedChart.NSeries[0].Marker.Area.ForegroundColor.ToArgb().ToString("X"));
}
}
}
```
### See Also
* class [Area](../../../aspose.cells.drawing/area/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
