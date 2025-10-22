##GlobalizationSettings.ChartSettings
GlobalizationSettings property. Gets or sets the globalization settings for Chart
## GlobalizationSettings.ChartSettings property
Gets or sets the globalization settings for Chart.
```csharp
public ChartGlobalizationSettings ChartSettings { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class CustomChartGlobalizationSettings : ChartGlobalizationSettings
{
public override string GetAxisUnitName(DisplayUnitType type)
{
switch (type)
{
case DisplayUnitType.Hundreds:
return "百";
case DisplayUnitType.Thousands:
return "千";
case DisplayUnitType.TenThousands:
return "万";
default:
return base.GetAxisUnitName(type);
}
}
}
public class GlobalizationSettingsPropertyChartSettingsDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Create a chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
Chart chart = sheet.Charts[chartIndex];
// Add sample data
chart.NSeries.Add("{10,20,30,40}", true);
// Set display units
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
chart.ValueAxis.IsDisplayUnitLabelShown = true;
Console.WriteLine("Default display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
// Apply custom globalization settings
wb.Settings.GlobalizationSettings = new GlobalizationSettings
{
ChartSettings = new CustomChartGlobalizationSettings()
};
// Verify the custom labels
Console.WriteLine("Custom display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
// Change display unit and verify
chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
Console.WriteLine("Updated display unit label: " + chart.ValueAxis.DisplayUnitLabel.Text);
}
}
}
```
### See Also
* class [ChartGlobalizationSettings](../../../aspose.cells.charts/chartglobalizationsettings/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
