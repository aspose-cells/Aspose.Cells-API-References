##ChartArea.Font
ChartArea property. Gets a Font object of the specified chartarea object
## ChartArea.Font property
Gets a `Font` object of the specified chartarea object.
```csharp
public override Font Font { get; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartAreaPropertyFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Region");
worksheet.Cells["A2"].PutValue("North");
worksheet.Cells["A3"].PutValue("South");
worksheet.Cells["A4"].PutValue("East");
worksheet.Cells["A5"].PutValue("West");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(5000);
worksheet.Cells["B3"].PutValue(3000);
worksheet.Cells["B4"].PutValue(4000);
worksheet.Cells["B5"].PutValue(6000);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Get chart area
ChartArea chartArea = chart.ChartArea;
// Set chart area font properties
Aspose.Cells.Font font = chartArea.Font;
font.Name = "Tahoma";
font.Size = 10;
font.Color = Color.Blue;
font.IsBold = true;
font.IsItalic = true;
font.Underline = FontUnderlineType.Single;
// Save the workbook
workbook.Save("ChartAreaFontDemo.xlsx");
}
}
}
```
### See Also
* class [Font](../../../aspose.cells/font/)
* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
