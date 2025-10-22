##DisplayUnitLabel.Text
DisplayUnitLabel property. Gets or sets the text of display unit label
## DisplayUnitLabel.Text property
Gets or sets the text of display unit label.
```csharp
public override string Text { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DisplayUnitLabelPropertyTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(1000);
worksheet.Cells["A2"].PutValue(2000);
worksheet.Cells["A3"].PutValue(3000);
worksheet.Cells["A4"].PutValue(4000);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("A1:A4", true);
// Configure display unit label
chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
chart.ValueAxis.IsDisplayUnitLabelShown = true;
// Access and modify the display unit label text
DisplayUnitLabel label = chart.ValueAxis.DisplayUnitLabel;
Console.WriteLine("Default Display Unit Label: " + label.Text);
// Change the text
label.Text = "K Units";
Console.WriteLine("Modified Display Unit Label: " + label.Text);
// Save the workbook
workbook.Save("DisplayUnitLabelDemo.xlsx");
}
}
}
```
### See Also
* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
