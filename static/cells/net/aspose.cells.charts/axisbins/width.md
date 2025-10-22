##AxisBins.Width
AxisBins property. Gets or sets the width of axis bin
## AxisBins.Width property
Gets or sets the width of axis bin
```csharp
public double Width { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisBinsPropertyWidthDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells["B1"].PutValue(10);
worksheet.Cells["C1"].PutValue(20);
worksheet.Cells["D1"].PutValue(15);
worksheet.Cells["B2"].PutValue(35);
worksheet.Cells["C2"].PutValue(32);
worksheet.Cells["D2"].PutValue(31);
// Create histogram chart
int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 7, 1, 25, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:D2", false);
chart.NSeries.CategoryData = "B1:D1";
// Set bin width
chart.CategoryAxis.Bins.Width = 12;
// Save and demonstrate the result
workbook.Save("AxisBinsPropertyWidthDemo_out.xlsx");
Console.WriteLine("Example executed successfully with bin width set to 12.");
}
}
}
```
### See Also
* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
