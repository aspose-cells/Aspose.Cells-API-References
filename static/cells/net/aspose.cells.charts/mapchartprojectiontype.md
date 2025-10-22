##Enum MapChartProjectionType
Aspose.Cells.Charts.MapChartProjectionType enum. Represents projection type of the map chart
## MapChartProjectionType enumeration
Represents projection type of the map chart.
```csharp
public enum MapChartProjectionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | Automatic |
| Mercator | `1` | Mercator |
| Miller | `2` | Miller |
| Albers | `3` | Albers |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class MapChartProjectionTypeDemo
{
public static void MapChartProjectionTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet for map chart
worksheet.Cells["A1"].PutValue("Country");
worksheet.Cells["A2"].PutValue("USA");
worksheet.Cells["A3"].PutValue("Canada");
worksheet.Cells["A4"].PutValue("Mexico");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(80);
worksheet.Cells["B4"].PutValue(60);
// Add a map chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set the chart data range
chart.SetChartDataRange("A1:B4", true);
// Set the projection type for the map chart
chart.NSeries[0].LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
// Output the projection type
Console.WriteLine("Map Chart Projection Type: " + chart.NSeries[0].LayoutProperties.MapChartProjectionType);
// Save the workbook
workbook.Save("MapChartProjectionTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
