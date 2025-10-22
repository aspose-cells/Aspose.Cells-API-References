##DataLabels.Area
DataLabels property. Gets the area
## DataLabels.Area property
Gets the `area`.
```csharp
public override Area Area { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyAreaDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells["A1"].PutValue(150);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(33);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(50);
// Create chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Scatter, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Configure data labels area
Series series = chart.NSeries[0];
series.DataLabels.ShowValue = true;
// Demonstrate Area property usage
series.DataLabels.Area.FillFormat.Pattern = FillPattern.Solid;
series.DataLabels.Area.BackgroundColor = Color.LightBlue;
series.DataLabels.Area.ForegroundColor = Color.White;
series.DataLabels.Area.Transparency = 0.3;
workbook.Save("DataLabelsAreaDemo.xlsx");
}
}
}
```
### See Also
* class [Area](../../../aspose.cells.drawing/area/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
