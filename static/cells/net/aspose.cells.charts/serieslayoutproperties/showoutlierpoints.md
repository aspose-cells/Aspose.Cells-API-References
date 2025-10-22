##SeriesLayoutProperties.ShowOutlierPoints
SeriesLayoutProperties property. Indicates whether showing outlier data points
## SeriesLayoutProperties.ShowOutlierPoints property
Indicates whether showing outlier data points.
```csharp
public bool ShowOutlierPoints { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesLayoutPropertiesPropertyShowOutlierPointsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(200); // Outlier value
worksheet.Cells["B1"].PutValue("Q1");
worksheet.Cells["B2"].PutValue("Q2");
worksheet.Cells["B3"].PutValue("Q3");
worksheet.Cells["B4"].PutValue("Q4");
// Create a column chart (which supports outlier points)
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series
chart.NSeries.Add("A1:A4", true);
chart.NSeries.CategoryData = "B1:B4";
// Configure series layout properties
Series series = chart.NSeries[0];
SeriesLayoutProperties layoutProperties = series.LayoutProperties;
// Demonstrate ShowOutlierPoints property
layoutProperties.ShowOutlierPoints = true;
layoutProperties.ShowInnerPoints = true;
layoutProperties.ShowMeanMarker = true;
workbook.Save("ChartWithOutliers.xlsx");
}
}
}
```
### See Also
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
