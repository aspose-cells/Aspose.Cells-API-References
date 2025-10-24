##TickLabels.Font
TickLabels property. Returns a Font object that represents the font of the specified TickLabels object
## TickLabels.Font property
Returns a `Font` object that represents the font of the specified TickLabels object.
```csharp
public Font Font { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TickLabelsPropertyFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category 1");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
worksheet.Cells["A4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("A2:A4", true);
chart.NSeries.CategoryData = "A1:A1";
// Access tick labels font
Aspose.Cells.Charts.TickLabels tickLabels = chart.CategoryAxis.TickLabels;
Font font = tickLabels.Font;
// Set font properties
font.Name = "Arial";
font.Size = 12;
font.IsBold = true;
// Save the workbook
workbook.Save("TickLabelsFontDemo.xlsx");
Console.WriteLine("TickLabels font properties set successfully.");
}
}
}
```
### See Also
* class [Font](../../../aspose.cells/font/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
