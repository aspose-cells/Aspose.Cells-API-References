##Class SeriesLayoutProperties
Aspose.Cells.Charts.SeriesLayoutProperties class. Represents the properties of series layout
## SeriesLayoutProperties class
Represents the properties of series layout.
```csharp
public class SeriesLayoutProperties
```
## Constructors
| Name | Description |
| --- | --- |
| [SeriesLayoutProperties](serieslayoutproperties/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [IsIntervalLeftClosed](../../aspose.cells.charts/serieslayoutproperties/isintervalleftclosed/) { get; set; } | Indicates whether the interval is closed on the left side. |
| [MapChartProjectionType](../../aspose.cells.charts/serieslayoutproperties/mapchartprojectiontype/) { get; set; } | Gets and sets the projection type of the map. |
| [MapChartRegionType](../../aspose.cells.charts/serieslayoutproperties/mapchartregiontype/) { get; set; } | Gets and sets the region type of the map. |
| [MapLabelLayout](../../aspose.cells.charts/serieslayoutproperties/maplabellayout/) { get; set; } | Gets and sets the layout of map labels. |
| [QuartileCalculation](../../aspose.cells.charts/serieslayoutproperties/quartilecalculation/) { get; set; } | Represents the statistical properties for the series. |
| [ShowConnectorLines](../../aspose.cells.charts/serieslayoutproperties/showconnectorlines/) { get; set; } | Indicates whether showing connector lines between data points. |
| [ShowInnerPoints](../../aspose.cells.charts/serieslayoutproperties/showinnerpoints/) { get; set; } | Indicates whether showing non-outlier data points. |
| [ShowMeanLine](../../aspose.cells.charts/serieslayoutproperties/showmeanline/) { get; set; } | Indicates whether showing the line connecting all mean points. |
| [ShowMeanMarker](../../aspose.cells.charts/serieslayoutproperties/showmeanmarker/) { get; set; } | Indicates whether showing markers denoting the mean. |
| [ShowOutlierPoints](../../aspose.cells.charts/serieslayoutproperties/showoutlierpoints/) { get; set; } | Indicates whether showing outlier data points. |
| [Subtotals](../../aspose.cells.charts/serieslayoutproperties/subtotals/) { get; set; } | Represents the index of a subtotal data point. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class SeriesLayoutPropertiesDemo
{
public static void SeriesLayoutPropertiesExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);
worksheet.Cells["C1"].PutValue("Q1");
worksheet.Cells["C2"].PutValue("Q2");
worksheet.Cells["C3"].PutValue("Y1");
worksheet.Cells["C4"].PutValue("Y2");
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add series to the chart
int seriesIndex = chart.NSeries.Add("A1:B4", true);
chart.NSeries.CategoryData = "C1:C4";
Series series = chart.NSeries[seriesIndex];
// Set the values of the series
series.Values = "=B1:B4";
// Access the SeriesLayoutProperties object
SeriesLayoutProperties layoutProperties = series.LayoutProperties;
// Set properties of SeriesLayoutProperties
layoutProperties.ShowConnectorLines = true;
layoutProperties.ShowMeanLine = true;
layoutProperties.ShowOutlierPoints = true;
layoutProperties.ShowMeanMarker = true;
layoutProperties.ShowInnerPoints = true;
layoutProperties.QuartileCalculation = QuartileCalculationType.Inclusive;
layoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
layoutProperties.IsIntervalLeftClosed = true;
layoutProperties.MapChartRegionType = MapChartRegionType.World;
layoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
// Save the workbook
workbook.Save("SeriesLayoutPropertiesExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
