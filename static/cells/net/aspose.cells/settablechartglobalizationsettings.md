##Class SettableChartGlobalizationSettings
Aspose.Cells.SettableChartGlobalizationSettings class. Implementation of PivotGlobalizationSettings that supports user to set/change predefined texts
## SettableChartGlobalizationSettings class
Implementation of PivotGlobalizationSettings that supports user to set/change pre-defined texts.
```csharp
public class SettableChartGlobalizationSettings : ChartGlobalizationSettings
```
## Constructors
| Name | Description |
| --- | --- |
| [SettableChartGlobalizationSettings](settablechartglobalizationsettings/)() | The default constructor. |
## Methods
| Name | Description |
| --- | --- |
| override [GetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/getaxistitlename/)() | Gets the name of Title for Axis. |
| override [GetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | Gets the Name of Axis Unit. |
| override [GetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/getcharttitlename/)() | Gets the name of Chart Title. |
| override [GetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/)() | Gets the name of Decrease for Legend. |
| override [GetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegendincreasename/)() | Gets the name of increase for Legend. |
| override [GetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/getlegendtotalname/)() | Gets the name of Total for Legend. |
| override [GetOtherName](../../aspose.cells/settablechartglobalizationsettings/getothername/)() | Gets the name of "Other" labels for Chart. |
| override [GetSeriesName](../../aspose.cells/settablechartglobalizationsettings/getseriesname/)() | Gets the name of Series in the Chart. |
| [SetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/setaxistitlename/)(string) | Sets the name of Title for Axis. |
| [SetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/setaxisunitname/)(DisplayUnitType, string) | Sets the Name of Axis Unit. |
| [SetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/setcharttitlename/)(string) | Sets the name of Chart Title. |
| [SetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/)(string) | Sets the name of Decrease for Legend. |
| [SetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegendincreasename/)(string) | Sets the name of increase for Legend. |
| [SetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/setlegendtotalname/)(string) | Sets the name of Total for Legend. |
| [SetOtherName](../../aspose.cells/settablechartglobalizationsettings/setothername/)(string) | Sets the name of "Other" labels for Chart. |
| [SetSeriesName](../../aspose.cells/settablechartglobalizationsettings/setseriesname/)(string) | Sets the name of Series in the Chart. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class CellsClassSettableChartGlobalizationSettingsDemo
{
public static void Run()
{
// Create a new workbook for demonstration
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Create an instance of SettableChartGlobalizationSettings
var settings = new SettableChartGlobalizationSettings();
// Set custom globalization settings
settings.SetSeriesName("Custom Series");
settings.SetChartTitleName("Custom Chart Title");
settings.SetLegendIncreaseName("Custom Increase");
settings.SetLegendDecreaseName("Custom Decrease");
// Create a custom GlobalizationSettings implementation
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings(settings);
// Create a simple chart to demonstrate the settings
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Q1");
worksheet.Cells["A3"].PutValue("Q2");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
chart.Title.Text = "Demo Chart";
Console.WriteLine("SettableChartGlobalizationSettings configured successfully");
workbook.Save("SettableChartGlobalizationSettingsDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error working with SettableChartGlobalizationSettings: {ex.Message}");
}
}
private class CustomGlobalizationSettings : GlobalizationSettings
{
private readonly SettableChartGlobalizationSettings _chartSettings;
public CustomGlobalizationSettings(SettableChartGlobalizationSettings chartSettings)
{
_chartSettings = chartSettings;
}
// Implement required GlobalizationSettings methods here
// that delegate to the SettableChartGlobalizationSettings instance
}
}
}
```
### See Also
* class [ChartGlobalizationSettings](../../aspose.cells.charts/chartglobalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
