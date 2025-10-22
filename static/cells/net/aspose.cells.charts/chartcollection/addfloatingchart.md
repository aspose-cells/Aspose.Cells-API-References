##ChartCollection.AddFloatingChart
ChartCollection method. Adds a chart to the collection
## ChartCollection.AddFloatingChart method
Adds a chart to the collection.
```csharp
public int AddFloatingChart(ChartType type, int left, int top, int width, int height)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ChartType | Chart type |
| left | Int32 | The x offset to corner |
| top | Int32 | The y offset to corner |
| width | Int32 | The chart width |
| height | Int32 | The chart height |
### Return Value
[`Chart`](../../chart/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartCollectionMethodAddFloatingChartWithChartTypeInt32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add floating chart with specified dimensions
int chartIndex = sheet.Charts.AddFloatingChart(ChartType.Column, 100, 100, 600, 400);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
// Add sample data to the chart
chart.NSeries.Add("{1,3,2,5}", false);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
