##Enum MapChartRegionType
Aspose.Cells.Charts.MapChartRegionType enum. Represents the region type of the map chart
## MapChartRegionType enumeration
Represents the region type of the map chart.
```csharp
public enum MapChartRegionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | Automatic |
| DataOnly | `1` | Only Data. |
| CountryRegionList | `2` | Country region list. |
| World | `3` | World. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class MapChartRegionTypeDemo
{
public static void MapChartRegionTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Country");
worksheet.Cells["A2"].PutValue("USA");
worksheet.Cells["A3"].PutValue("Canada");
worksheet.Cells["A4"].PutValue("Mexico");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
// Add a map chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set the chart data range
chart.SetChartDataRange("A1:B4", true);
// Set the region type of the map chart
foreach (Series series in chart.NSeries)
{
series.LayoutProperties.MapChartRegionType = MapChartRegionType.CountryRegionList;
}
// Save the workbook
workbook.Save("MapChartRegionTypeExample.xlsx");
// Output the result
Console.WriteLine("Map chart with region type 'CountryRegionList' created successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
