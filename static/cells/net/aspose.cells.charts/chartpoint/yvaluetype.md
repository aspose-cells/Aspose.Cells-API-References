##ChartPoint.YValueType
ChartPoint property. Gets Y value type of the chart point
## ChartPoint.YValueType property
Gets Y value type of the chart point.
```csharp
public CellValueType YValueType { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyYValueTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the first chart point in the first series
ChartPoint chartPoint = chart.NSeries[0].Points[0];
// Display the current YValueType
Console.WriteLine("Current YValueType: " + chartPoint.YValueType);
// Display the YValue before change
Console.WriteLine("Current YValue: " + chartPoint.YValue);
// Change the YValue to a different type (string to demonstrate type change)
chartPoint.YValue = "15"; // This will change the YValueType to IsString
// Display the YValueType after change
Console.WriteLine("New YValueType: " + chartPoint.YValueType);
Console.WriteLine("New YValue: " + chartPoint.YValue);
// Save the workbook
workbook.Save("ChartPointPropertyYValueTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
