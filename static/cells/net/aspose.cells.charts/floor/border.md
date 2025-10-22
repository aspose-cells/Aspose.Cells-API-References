##Floor.Border
Floor property. Gets or sets the border Line
## Floor.Border property
Gets or sets the border [`Line`](../../../aspose.cells.drawing/line/).
```csharp
public Line Border { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class FloorPropertyBorderDemo
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
// Add a 3D column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the floor of the chart
Floor floor = chart.Floor;
// Set border properties by modifying existing border rather than creating new one
floor.Border.Color = Color.Red;
floor.Border.Weight = WeightType.MediumLine;
floor.Border.DashType = MsoLineDashStyle.DashDot;
floor.Border.IsVisible = true;
floor.Border.Transparency = 0.5;
// Save the workbook
workbook.Save("FloorBorderDemo.xlsx");
}
}
}
```
### See Also
* class [Line](../../../aspose.cells.drawing/line/)
* class [Floor](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
