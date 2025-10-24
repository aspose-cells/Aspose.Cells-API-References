##SeriesLayoutProperties.MapLabelLayout
SeriesLayoutProperties property. Gets and sets the layout of map labels
## SeriesLayoutProperties.MapLabelLayout property
Gets and sets the layout of map labels.
```csharp
public MapChartLabelLayout MapLabelLayout { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesLayoutPropertiesPropertyMapLabelLayoutDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for map chart
worksheet.Cells["A1"].PutValue("Country");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("United States");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("Canada");
worksheet.Cells["B3"].PutValue(80);
worksheet.Cells["A4"].PutValue("Mexico");
worksheet.Cells["B4"].PutValue(60);
// Add a map chart
int chartIndex = worksheet.Charts.Add(ChartType.Map, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
Series series = chart.NSeries[0];
series.XValues = "A2:A4";
// Configure map layout properties
series.LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
series.LayoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
series.LayoutProperties.MapChartRegionType = MapChartRegionType.DataOnly;
// Save the workbook
workbook.Save("MapLabelLayoutDemo.xlsx");
}
}
}
```
### See Also
* enum [MapChartLabelLayout](../../mapchartlabellayout/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
