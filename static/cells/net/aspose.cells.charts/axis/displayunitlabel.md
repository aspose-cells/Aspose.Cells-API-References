##Axis.DisplayUnitLabel
Axis property. Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values for example in the millions or billions
## Axis.DisplayUnitLabel property
Represents a unit label on an axis in the specified chart. Unit labels are useful for charting large values— for example, in the millions or billions.
```csharp
public DisplayUnitLabel DisplayUnitLabel { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyDisplayUnitLabelDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(1000);
worksheet.Cells["A2"].PutValue(2000);
worksheet.Cells["A3"].PutValue(3000);
worksheet.Cells["A4"].PutValue(4000);
// Create chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("A1:A4", true);
// Configure display unit and label
chart.ValueAxis.DisplayUnit = Aspose.Cells.Charts.DisplayUnitType.Thousands;
chart.ValueAxis.IsDisplayUnitLabelShown = true;
// Output the display unit label text
Console.WriteLine("Display Unit Label: " + chart.ValueAxis.DisplayUnitLabel.Text);
// Save the workbook
workbook.Save("AxisPropertyDisplayUnitLabelDemo_out.xlsx");
}
}
}
```
### See Also
* class [DisplayUnitLabel](../../displayunitlabel/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
