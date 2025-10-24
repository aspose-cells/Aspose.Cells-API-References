##SettableChartGlobalizationSettings.GetSeriesName
SettableChartGlobalizationSettings method. Gets the name of Series in the Chart
## SettableChartGlobalizationSettings.GetSeriesName method
Gets the name of Series in the Chart.
```csharp
public override string GetSeriesName()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class SettableChartGlobalizationSettingsMethodGetSeriesNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Series");
worksheet.Cells["A2"].PutValue("Category 1");
worksheet.Cells["A3"].PutValue("Category 2");
worksheet.Cells["B1"].PutValue("Column A");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["C1"].PutValue("Column B");
worksheet.Cells["C2"].PutValue(150);
worksheet.Cells["C3"].PutValue(250);
// Create a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Create and apply globalization settings
SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();
settings.SetSeriesName("Custom Series Name");
// The globalization settings are used when rendering/displaying the chart,
// but not directly assigned to the chart object
// (as the Chart class doesn't have this property)
try
{
// Get the customized series name
string seriesName = settings.GetSeriesName();
Console.WriteLine("Series Name: " + seriesName);
// Save the workbook
workbook.Save("MethodGetSeriesNameDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetSeriesName method: {ex.Message}");
}
}
}
}
```
### See Also
* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
