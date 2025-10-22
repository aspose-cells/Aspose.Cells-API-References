##Series.Name
Series property. Gets or sets the name of the data series
## Series.Name property
Gets or sets the name of the data series.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Series Name");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["C2"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add series to the chart
chart.NSeries.Add("A2:C2", true);
// Demonstrate Name property usage
// 1. Reference name to a cell
chart.NSeries[0].Name = "=A1";
// 2. Set a string to name
chart.NSeries[0].Name = "First Series";
// Save the workbook
workbook.Save("SeriesPropertyNameDemo_out.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
