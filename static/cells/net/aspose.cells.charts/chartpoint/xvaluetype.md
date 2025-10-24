##ChartPoint.XValueType
ChartPoint property. Gets X value type of the chart point
## ChartPoint.XValueType property
Gets X value type of the chart point.
```csharp
public CellValueType XValueType { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointPropertyXValueTypeDemo
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
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the first chart point
ChartPoint point = chart.NSeries[0].Points[0];
// Display the current XValueType
Console.WriteLine("Current XValueType: " + point.XValueType);
// Set new XValue (this will automatically update XValueType)
point.XValue = DateTime.Now; // Changing to DateTime type
Console.WriteLine("After setting DateTime value, XValueType: " + point.XValueType);
point.XValue = "New Category"; // Changing to String type
Console.WriteLine("After setting String value, XValueType: " + point.XValueType);
point.XValue = 123.45; // Changing to Numeric type
Console.WriteLine("After setting Numeric value, XValueType: " + point.XValueType);
// Save the workbook
workbook.Save("ChartPointXValueTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
