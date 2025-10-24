##SeriesLayoutProperties.ShowMeanLine
SeriesLayoutProperties property. Indicates whether showing the line connecting all mean points
## SeriesLayoutProperties.ShowMeanLine property
Indicates whether showing the line connecting all mean points.
```csharp
public bool ShowMeanLine { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesLayoutPropertiesPropertyShowMeanLineDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for box and whisker chart
worksheet.Cells["A1"].PutValue("Series 1");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(40);
worksheet.Cells["A4"].PutValue(25);
worksheet.Cells["A5"].PutValue(40);
worksheet.Cells["A6"].PutValue(115);
worksheet.Cells["A7"].PutValue(65.666);
// Add a box and whisker chart
int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series to the chart
chart.NSeries.Add("A1:A7", true);
// Get the first series
Series series = chart.NSeries[0];
// Access layout properties
SeriesLayoutProperties layout = series.LayoutProperties;
// Demonstrate ShowMeanLine property
Console.WriteLine("Default ShowMeanLine value: " + layout.ShowMeanLine);
// Set ShowMeanLine to true
layout.ShowMeanLine = true;
Console.WriteLine("After setting ShowMeanLine to true: " + layout.ShowMeanLine);
// Save the workbook
workbook.Save("BoxWhiskerChart_ShowMeanLineDemo.xlsx");
}
}
}
```
### See Also
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
