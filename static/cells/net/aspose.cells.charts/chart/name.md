##Chart.Name
Chart property. Gets and sets the name of the chart
## Chart.Name property
Gets and sets the name of the chart.
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
public class ChartPropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Display chart name
Console.WriteLine("Chart Name: " + chart.Name);
// Add another chart and display its name
int chartIndex2 = worksheet.Charts.Add(ChartType.Pie, 20, 0, 30, 5);
Aspose.Cells.Charts.Chart chart2 = worksheet.Charts[chartIndex2];
chart2.NSeries.Add("B2:B4", true);
chart2.NSeries.CategoryData = "A2:A4";
Console.WriteLine("Second Chart Name: " + chart2.Name);
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
