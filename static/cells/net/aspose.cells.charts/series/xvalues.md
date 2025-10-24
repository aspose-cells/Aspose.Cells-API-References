##Series.XValues
Series property. Represents the x values of the chart series
## Series.XValues property
Represents the x values of the chart series.
```csharp
public string XValues { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyXValuesDemo
{
public static void Run()
{
// Create a new workbook
var workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("X Values");
worksheet.Cells["B1"].PutValue("Series 1");
worksheet.Cells["C1"].PutValue("Series 2");
for (int i = 0; i < 5; i++)
{
worksheet.Cells[i+1, 0].PutValue(i+1); // X values 1-5
worksheet.Cells[i+1, 1].PutValue((i+1)*2); // Series 1 values
worksheet.Cells[i+1, 2].PutValue((i+1)*3); // Series 2 values
}
// Add a scatter chart
int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Add series with XValues and Values
int seriesIndex = chart.NSeries.Add("B2:B6", false);
Series series = chart.NSeries[seriesIndex];
series.XValues = "A2:A6"; // Demonstrating XValues property
series.Name = "Series 1";
seriesIndex = chart.NSeries.Add("C2:C6", false);
series = chart.NSeries[seriesIndex];
series.XValues = "A2:A6"; // Demonstrating XValues property again
series.Name = "Series 2";
// Save the workbook
workbook.Save("SeriesXValuesDemo.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
