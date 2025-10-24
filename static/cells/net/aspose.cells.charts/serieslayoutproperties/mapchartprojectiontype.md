##SeriesLayoutProperties.MapChartProjectionType
SeriesLayoutProperties property. Gets and sets the projection type of the map
## SeriesLayoutProperties.MapChartProjectionType property
Gets and sets the projection type of the map.
```csharp
public MapChartProjectionType MapChartProjectionType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesLayoutPropertiesPropertyMapChartProjectionTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Country");
worksheet.Cells["A2"].PutValue("USA");
worksheet.Cells["A3"].PutValue("Canada");
worksheet.Cells["A4"].PutValue("Mexico");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(80);
worksheet.Cells["B4"].PutValue(60);
int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
chart.NSeries[0].LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
Console.WriteLine("Map Chart Projection Type: " + chart.NSeries[0].LayoutProperties.MapChartProjectionType);
workbook.Save("MapChartProjectionTypeExample.xlsx");
}
}
}
```
### See Also
* enum [MapChartProjectionType](../../mapchartprojectiontype/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
