##Series.BubbleScale
Series property. Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 zero to 300 corresponding to a percentage of the default size. Applies only to bubble charts
## Series.BubbleScale property
Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts.
```csharp
public int BubbleScale { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SeriesPropertyBubbleScaleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for bubble chart
worksheet.Cells["A1"].PutValue("X");
worksheet.Cells["B1"].PutValue("Y");
worksheet.Cells["C1"].PutValue("Size");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["C2"].PutValue(5);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["C3"].PutValue(10);
worksheet.Cells["A4"].PutValue(3);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["C4"].PutValue(15);
// Add a bubble chart
int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Add series to the chart
int seriesIndex = chart.NSeries.Add("B2:B4", true);
chart.NSeries[seriesIndex].XValues = "A2:A4";
chart.NSeries[seriesIndex].BubbleSizes = "C2:C4";
// Set bubble scale to demonstrate the property
chart.NSeries[seriesIndex].BubbleScale = 150; // Scale bubbles to 150% of default size
// Customize the chart appearance
chart.Title.Text = "Bubble Chart with Scaled Bubbles";
chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.LightBlue, 0.5, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 1);
// Save the workbook
workbook.Save("BubbleScaleDemo.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
