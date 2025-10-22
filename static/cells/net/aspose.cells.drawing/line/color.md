##Line.Color
Line property. Represents the Color of the line
## Line.Color property
Represents the Color of the line.
```csharp
public Color Color { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class LinePropertyColorDemo
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
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set axis line colors
chart.CategoryAxis.AxisLine.Color = Color.BlueViolet;
chart.ValueAxis.AxisLine.Color = Color.BlueViolet;
// Set axis title font color
chart.CategoryAxis.Title.Text = "Categories";
chart.CategoryAxis.Title.Font.Color = Color.BlueViolet;
// Save the workbook
workbook.Save("LinePropertyColorDemo_out.xlsx");
}
}
}
```
### See Also
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
