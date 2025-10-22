##SeriesLayoutProperties.ShowConnectorLines
SeriesLayoutProperties property. Indicates whether showing connector lines between data points
## SeriesLayoutProperties.ShowConnectorLines property
Indicates whether showing connector lines between data points.
```csharp
public bool ShowConnectorLines { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesLayoutPropertiesPropertyShowConnectorLinesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);
// Add chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
int seriesIndex = chart.NSeries.Add("A1:B4", true);
Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
// Set ShowConnectorLines and other properties
Aspose.Cells.Charts.SeriesLayoutProperties layoutProperties = series.LayoutProperties;
layoutProperties.ShowConnectorLines = true;
layoutProperties.ShowMeanLine = true;
workbook.Save("SeriesLayoutPropertiesShowConnectorLinesDemo.xlsx");
}
}
}
```
### See Also
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
