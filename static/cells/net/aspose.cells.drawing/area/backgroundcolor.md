##Area.BackgroundColor
Area property. Gets or sets the background Color of the Area
## Area.BackgroundColor property
Gets or sets the background Color of the [`Area`](../).
```csharp
public Color BackgroundColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class AreaPropertyBackgroundColorDemo
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
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// Set background color for category axis area
chart.CategoryAxis.Area.BackgroundColor = System.Drawing.Color.Red;
// Display the background color
Console.WriteLine("Category Axis Background Color: " + chart.CategoryAxis.Area.BackgroundColor);
// Save the workbook
workbook.Save("AreaPropertyBackgroundColorDemo_out.xlsx");
}
}
}
```
### See Also
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
