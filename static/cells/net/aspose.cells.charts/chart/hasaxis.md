##Chart.HasAxis
Chart method. Returns which axes exist on the chart
## Chart.HasAxis method
Returns which axes exist on the chart.
```csharp
public bool HasAxis(AxisType aixsType, bool isPrimary)
```
### Remarks
Normally, Pie, PieExploded, PiePie,PieBar, Pie3D, Pie3DExploded,Doughnut, DoughnutExploded is no axis.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartMethodHasAxisWithAxisTypeBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
bool hasPrimaryValueAxis = chart.HasAxis(Aspose.Cells.Charts.AxisType.Value, true);
bool hasSecondaryValueAxis = chart.HasAxis(Aspose.Cells.Charts.AxisType.Value, false);
Console.WriteLine("Primary Value Axis exists: " + hasPrimaryValueAxis);
Console.WriteLine("Secondary Value Axis exists: " + hasSecondaryValueAxis);
workbook.Save("ChartHasAxisDemo.xlsx");
}
}
}
```
### See Also
* enum [AxisType](../../axistype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
