##ChartGlobalizationSettings.GetSeriesName
ChartGlobalizationSettings method. Gets the name of Series in the Chart
## ChartGlobalizationSettings.GetSeriesName method
Gets the name of Series in the Chart.
```csharp
public virtual string GetSeriesName()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartGlobalizationSettingsMethodGetSeriesNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category 1");
worksheet.Cells["A2"].PutValue("Category 2");
worksheet.Cells["A3"].PutValue("Category 3");
worksheet.Cells["B1"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(30);
// Add a chart and set data
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B1:B3", true);
chart.NSeries.CategoryData = "A1:A3";
// Create globalization settings and get series name
Aspose.Cells.Charts.ChartGlobalizationSettings globalizationSettings = new Aspose.Cells.Charts.ChartGlobalizationSettings();
string seriesName = globalizationSettings.GetSeriesName();
// Output the result
Console.WriteLine("Series Name: " + seriesName);
// Save the workbook
workbook.Save("ChartGlobalizationSettingsExample.xlsx");
}
}
}
```
### See Also
* class [ChartGlobalizationSettings](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
