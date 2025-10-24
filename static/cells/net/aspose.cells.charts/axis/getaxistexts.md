##Axis.GetAxisTexts
Axis method. Gets the labels of the axis after call Chart.Calculate method
## Axis.GetAxisTexts method
Gets the labels of the axis after call Chart.Calculate() method.
```csharp
public string[] GetAxisTexts()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisMethodGetAxisTextsDemo
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
worksheet.Cells["B2"].PutValue(8000);
worksheet.Cells["B3"].PutValue(4000);
worksheet.Cells["B4"].PutValue(-8000);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart
chart.Calculate();
// Get axis labels
string[] labels = chart.ValueAxis.GetAxisTexts();
// Output the labels
Console.WriteLine("Value Axis Labels:");
foreach (string label in labels)
{
Console.WriteLine(label);
}
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
