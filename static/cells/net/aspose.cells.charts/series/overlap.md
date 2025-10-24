##Series.Overlap
Series property. Specifies how bars and columns are positioned. Can be a value between  100 and 100. Applies only to 2D bar and 2D column charts
## Series.Overlap property
Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts.
```csharp
public short Overlap { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyOverlapDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for chart
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["A3"].PutValue("B");
sheet.Cells["A4"].PutValue("C");
sheet.Cells["B1"].PutValue("Series1");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(30);
sheet.Cells["C1"].PutValue("Series2");
sheet.Cells["C2"].PutValue(15);
sheet.Cells["C3"].PutValue(25);
sheet.Cells["C4"].PutValue(35);
// Add a clustered column chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set overlap property for the first series
chart.NSeries[0].Overlap = -40;
// Save the workbook
workbook.Save("SeriesOverlapDemo.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
