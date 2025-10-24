##ChartPoint.Area
ChartPoint property. Gets the  area
## ChartPoint.Area property
Gets the ` area`.
```csharp
public Area Area { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ChartPointPropertyAreaDemo
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
sheet.Cells["A5"].PutValue("D");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(30);
sheet.Cells["B5"].PutValue(40);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Access the first point in the first series and set area properties
Aspose.Cells.Charts.ChartPoint point = chart.NSeries[0].Points[0];
point.Area.ForegroundColor = System.Drawing.Color.Red;
point.Area.FillFormat.Texture = TextureType.Granite;
point.Area.Formatting = FormattingType.Custom;
// Save the workbook
workbook.Save("ChartPointAreaDemo.xlsx");
}
}
}
```
### See Also
* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
