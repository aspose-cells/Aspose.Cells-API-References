##Chart.Calculate
Chart method. Calculates the custom position of plot area axes if the position of them are auto assigned
## Calculate() {#calculate}
Calculates the custom position of plot area, axes if the position of them are auto assigned.
```csharp
public void Calculate()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartMethodCalculateDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate the chart before saving
chart.Calculate();
// Save the workbook with chart
workbook.Save("ChartCalculateDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
## Calculate(ChartCalculateOptions) {#calculate_1}
Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options.
```csharp
public void Calculate(ChartCalculateOptions calculateOptions)
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartMethodCalculateWithChartCalculateOptionsDemo
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
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(150);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Enable data labels
chart.NSeries[0].DataLabels.ShowValue = true;
// Create calculate options and set to update all points
ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
calculateOptions.UpdateAllPoints = true;
// Calculate chart with options
chart.Calculate(calculateOptions);
// Output the data label texts
ChartPointCollection points = chart.NSeries[0].Points;
Console.WriteLine("DataLabel Text for Point 0: " + points[0].DataLabels.Text);
Console.WriteLine("DataLabel Text for Point 1: " + points[1].DataLabels.Text);
Console.WriteLine("DataLabel Text for Point 2: " + points[2].DataLabels.Text);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ChartCalculateOptions](../../chartcalculateoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
