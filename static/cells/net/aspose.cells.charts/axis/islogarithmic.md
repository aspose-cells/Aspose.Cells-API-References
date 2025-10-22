##Axis.IsLogarithmic
Axis property. Represents if the value axis scale type is logarithmic or not
## Axis.IsLogarithmic property
Represents if the value axis scale type is logarithmic or not.
```csharp
public bool IsLogarithmic { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyIsLogarithmicDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(1);
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(100);
worksheet.Cells["A4"].PutValue(1000);
worksheet.Cells["B1"].PutValue(5);
worksheet.Cells["B2"].PutValue(25);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(100);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Add series
chart.NSeries.Add("A1:A4", true);
chart.NSeries[0].Values = "B1:B4";
// Configure logarithmic axis
chart.CategoryAxis.IsLogarithmic = true;
chart.CategoryAxis.LogBase = 10;
chart.CategoryAxis.MinValue = 1;
chart.CategoryAxis.MaxValue = 10000;
// Save the workbook
workbook.Save("AxisPropertyIsLogarithmicDemo_out.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
