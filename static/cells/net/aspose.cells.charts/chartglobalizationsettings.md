##Class ChartGlobalizationSettings
Aspose.Cells.Charts.ChartGlobalizationSettings class. Represents the globalization settings for chart
## ChartGlobalizationSettings class
Represents the globalization settings for chart.
```csharp
public class ChartGlobalizationSettings
```
## Constructors
| Name | Description |
| --- | --- |
| [ChartGlobalizationSettings](chartglobalizationsettings/)() | The default constructor. |
## Methods
| Name | Description |
| --- | --- |
| virtual [GetAxisTitleName](../../aspose.cells.charts/chartglobalizationsettings/getaxistitlename/)() | Gets the name of Title for Axis. |
| virtual [GetAxisUnitName](../../aspose.cells.charts/chartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | Gets the Name of Axis Unit. |
| virtual [GetChartTitleName](../../aspose.cells.charts/chartglobalizationsettings/getcharttitlename/)() | Gets the name of Chart Title. |
| virtual [GetLegendDecreaseName](../../aspose.cells.charts/chartglobalizationsettings/getlegenddecreasename/)() | Gets the name of Decrease for Legend. |
| virtual [GetLegendIncreaseName](../../aspose.cells.charts/chartglobalizationsettings/getlegendincreasename/)() | Gets the name of increase for Legend. |
| virtual [GetLegendTotalName](../../aspose.cells.charts/chartglobalizationsettings/getlegendtotalname/)() | Gets the name of Total for Legend. |
| virtual [GetOtherName](../../aspose.cells.charts/chartglobalizationsettings/getothername/)() | Gets the name of "Other" labels for Chart. |
| virtual [GetSeriesName](../../aspose.cells.charts/chartglobalizationsettings/getseriesname/)() | Gets the name of Series in the Chart. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartGlobalizationSettingsDemo
{
public static void ChartGlobalizationSettingsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category 1");
worksheet.Cells["A2"].PutValue("Category 2");
worksheet.Cells["A3"].PutValue("Category 3");
worksheet.Cells["B1"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(30);
chart.NSeries.Add("B1:B3", true);
chart.NSeries.CategoryData = "A1:A3";
// Create an instance of ChartGlobalizationSettings
ChartGlobalizationSettings globalizationSettings = new ChartGlobalizationSettings();
// Demonstrate the usage of methods in ChartGlobalizationSettings
string seriesName = globalizationSettings.GetSeriesName();
string chartTitleName = globalizationSettings.GetChartTitleName();
string legendIncreaseName = globalizationSettings.GetLegendIncreaseName();
string legendDecreaseName = globalizationSettings.GetLegendDecreaseName();
string legendTotalName = globalizationSettings.GetLegendTotalName();
string axisTitleName = globalizationSettings.GetAxisTitleName();
string otherName = globalizationSettings.GetOtherName();
string axisUnitName = globalizationSettings.GetAxisUnitName(DisplayUnitType.Thousands);
// Print the retrieved names to the console
Console.WriteLine("Series Name: " + seriesName);
Console.WriteLine("Chart Title Name: " + chartTitleName);
Console.WriteLine("Legend Increase Name: " + legendIncreaseName);
Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);
Console.WriteLine("Legend Total Name: " + legendTotalName);
Console.WriteLine("Axis Title Name: " + axisTitleName);
Console.WriteLine("Other Name: " + otherName);
Console.WriteLine("Axis Unit Name: " + axisUnitName);
// Save the workbook
workbook.Save("ChartGlobalizationSettingsExample.xlsx");
workbook.Save("ChartGlobalizationSettingsExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
