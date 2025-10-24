##Series.SplitValue
Series property. Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart
## Series.SplitValue property
Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.
```csharp
public double SplitValue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertySplitValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["A5"].PutValue("Grape");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(15);
worksheet.Cells["B3"].PutValue(25);
worksheet.Cells["B4"].PutValue(10);
worksheet.Cells["B5"].PutValue(50);
// Add a pie chart
int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Set split type and value
chart.NSeries[0].SplitType = ChartSplitType.Custom;
chart.NSeries[0].SplitValue = 20; // Split points with value <= 20
// Save the workbook
workbook.Save("SeriesPropertySplitValueDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
