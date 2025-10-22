##SeriesCollection.CategoryData
SeriesCollection property. Gets or sets the range of category Axis values. It can be a range of cells such as d1e10 or a sequence of values such as26810
## SeriesCollection.CategoryData property
Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}").
```csharp
public string CategoryData { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesCollectionPropertyCategoryDataDemo
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
for (int i = 2; i <= 10; i++)
{
worksheet.Cells["A" + i].PutValue("Cat " + (i - 1));
worksheet.Cells["B" + i].PutValue(i * 10);
}
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("=Sheet1!$B$2:$B$10", true);
chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$10";
// Save the workbook
workbook.Save("CategoryDataDemo.xlsx");
// Verify the CategoryData property
Console.WriteLine("Chart CategoryData: " + chart.NSeries.CategoryData);
}
}
}
```
### See Also
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
