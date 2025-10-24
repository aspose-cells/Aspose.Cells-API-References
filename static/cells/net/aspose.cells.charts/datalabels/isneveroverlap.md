##DataLabels.IsNeverOverlap
DataLabels property. Indicates whether the datalabels display never overlap. For Pie chart
## DataLabels.IsNeverOverlap property
Indicates whether the datalabels display never overlap. (For Pie chart)
```csharp
public bool IsNeverOverlap { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyIsNeverOverlapDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Enable data labels
Series series = chart.NSeries[0];
series.DataLabels.ShowValue = true;
// Get data labels and set IsNeverOverlap property
DataLabels dataLabels = series.DataLabels;
Console.WriteLine("Default IsNeverOverlap value: " + dataLabels.IsNeverOverlap);
// Set IsNeverOverlap to true
dataLabels.IsNeverOverlap = true;
Console.WriteLine("After setting IsNeverOverlap: " + dataLabels.IsNeverOverlap);
// Save the workbook
workbook.Save("DataLabelsIsNeverOverlapDemo.xlsx");
}
}
}
```
### See Also
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
