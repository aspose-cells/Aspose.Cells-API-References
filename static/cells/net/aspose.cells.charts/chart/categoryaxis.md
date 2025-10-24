##Chart.CategoryAxis
Chart property. Gets the charts X axis
## Chart.CategoryAxis property
Gets the chart's X axis.
```csharp
public Axis CategoryAxis { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyCategoryAxisDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for the chart
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["A3"].PutValue("B");
sheet.Cells["A4"].PutValue("C");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(30);
// Add a column chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access and modify CategoryAxis properties
chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;
chart.CategoryAxis.Title.Text = "Sample Categories";
chart.CategoryAxis.Title.Font.Size = 12;
// Save the workbook
workbook.Save("CategoryAxisDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
