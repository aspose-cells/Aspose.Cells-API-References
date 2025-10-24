##Chart.Is3D
Chart property. Indicates whether the chart is a 3d chart
## Chart.Is3D property
Indicates whether the chart is a 3d chart.
```csharp
public bool Is3D { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPropertyIs3DDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Q1");
worksheet.Cells["A3"].PutValue("Q2");
worksheet.Cells["A4"].PutValue("Q3");
worksheet.Cells["A5"].PutValue("Q4");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1200);
worksheet.Cells["B3"].PutValue(1500);
worksheet.Cells["B4"].PutValue(1800);
worksheet.Cells["B5"].PutValue(2100);
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 6, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set data range for the chart
chart.SetChartDataRange("A1:B5", true);
// Display the current Is3D value
Console.WriteLine("Current Is3D value: " + chart.Is3D);
// Create a 3D version of the chart
int chart3DIndex = worksheet.Charts.Add(ChartType.Column3D, 6, 12, 20, 22);
Chart chart3D = worksheet.Charts[chart3DIndex];
chart3D.SetChartDataRange("A1:B5", true);
// Display the 3D chart's Is3D value
Console.WriteLine("3D Chart Is3D value: " + chart3D.Is3D);
// Save the workbook
workbook.Save("ChartPropertyIs3DDemo.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
