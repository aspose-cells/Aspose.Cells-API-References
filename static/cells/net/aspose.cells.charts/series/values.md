##Series.Values
Series property. Represents the Y values of this chart series
## Series.Values property
Represents the Y values of this chart series.
```csharp
public string Values { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyValuesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Series1");
worksheet.Cells["C1"].PutValue("Series2");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["C2"].PutValue(15);
worksheet.Cells["C3"].PutValue(25);
worksheet.Cells["C4"].PutValue(35);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add series using the Values property
chart.NSeries.Add("=Sheet1!$B$2:$B$4", true);
chart.NSeries.Add("=Sheet1!$C$2:$C$4", true);
// Set category data
chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";
// Display the Values property for each series
Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
Console.WriteLine("Series 2 Values: " + chart.NSeries[1].Values);
// Save the workbook
workbook.Save("SeriesPropertyValuesDemo.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
