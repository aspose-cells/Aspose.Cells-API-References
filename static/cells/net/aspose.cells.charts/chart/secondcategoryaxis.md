##Chart.SecondCategoryAxis
Chart property. Gets the charts second X axis
## Chart.SecondCategoryAxis property
Gets the chart's second X axis.
```csharp
public Axis SecondCategoryAxis { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertySecondCategoryAxisDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Series 1");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["C1"].PutValue("Series 2");
worksheet.Cells["C2"].PutValue(15);
worksheet.Cells["C3"].PutValue(25);
worksheet.Cells["C4"].PutValue(35);
// Add a chart with secondary axis
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series to the chart
chart.NSeries.Add("B2:B4", true);
chart.NSeries.Add("C2:C4", true);
chart.NSeries.CategoryData = "A2:A4";
// Enable secondary category axis
chart.SecondCategoryAxis.IsVisible = true;
chart.SecondCategoryAxis.Title.Text = "Secondary Category Axis";
// Set some properties of the secondary category axis
chart.SecondCategoryAxis.MajorTickMark = TickMarkType.Cross;
chart.SecondCategoryAxis.MinorTickMark = TickMarkType.Outside;
chart.SecondCategoryAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;
// Save the workbook
workbook.Save("SecondCategoryAxisDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
