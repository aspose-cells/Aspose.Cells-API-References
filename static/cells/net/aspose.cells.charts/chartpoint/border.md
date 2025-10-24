##ChartPoint.Border
ChartPoint property. Gets the  border
## ChartPoint.Border property
Gets the [` border`](../../../aspose.cells.drawing/line/).
```csharp
public Line Border { get; }
```
### Examples
```csharp
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPointPropertyBorderDemo
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
int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
ChartPointCollection points = chart.NSeries[0].Points;
for (int i = 0; i < points.Count; i++)
{
points[i].Explosion = 15;
points[i].Border.Color = Color.Red;
}
workbook.Save("ChartPointPropertyBorderDemo.xlsx");
}
}
}
```
### See Also
* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
