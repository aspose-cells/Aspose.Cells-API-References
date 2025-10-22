##DataLabels.Number
DataLabels property. Gets and sets the builtin number format
## DataLabels.Number property
Gets and sets the built-in number format.
```csharp
public int Number { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyNumberDemo
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
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Bar, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the first series and enable data labels
Series series = chart.NSeries[0];
series.DataLabels.ShowValue = true;
// Access data labels properties
DataLabels dataLabels = series.DataLabels;
// Demonstrate Number property usage
Console.WriteLine("Original Number format: " + dataLabels.NumberFormat);
Console.WriteLine("Original Number property value: " + dataLabels.Number);
// Change the number format
dataLabels.Number = 2; // Currency format
dataLabels.NumberFormat = "$#,##0.00";
Console.WriteLine("Modified Number format: " + dataLabels.NumberFormat);
Console.WriteLine("Modified Number property value: " + dataLabels.Number);
// Save the workbook
workbook.Save("DataLabelsNumberDemo.xlsx");
}
}
}
```
### See Also
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
