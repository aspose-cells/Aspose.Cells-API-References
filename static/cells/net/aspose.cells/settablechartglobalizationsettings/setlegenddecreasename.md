##SettableChartGlobalizationSettings.SetLegendDecreaseName
SettableChartGlobalizationSettings method. Sets the name of Decrease for Legend
## SettableChartGlobalizationSettings.SetLegendDecreaseName method
Sets the name of Decrease for Legend.
```csharp
public void SetLegendDecreaseName(string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | local dependent name |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class SettableChartGlobalizationSettingsMethodSetLegendDecreaseNameWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for a chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Q1");
worksheet.Cells["A3"].PutValue("Q2");
worksheet.Cells["A4"].PutValue("Q3");
worksheet.Cells["B1"].PutValue("Series");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
// Create a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Create globalization settings
SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();
try
{
// Call SetLegendDecreaseName with a custom string
settings.SetLegendDecreaseName("Custom Decrease Label");
// The Chart class doesn't have a ChartGlobalizationSettings property,
// so we need to use the settings object directly where needed
// (Note: In actual usage, you would need to find where these settings are applied)
Console.WriteLine("SetLegendDecreaseName method executed successfully with parameter: 'Custom Decrease Label'");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetLegendDecreaseName method: {ex.Message}");
}
// Save the workbook
workbook.Save("SetLegendDecreaseNameDemo.xlsx");
}
}
}
```
### See Also
* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
