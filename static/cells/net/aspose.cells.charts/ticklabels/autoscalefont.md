##TickLabels.AutoScaleFont
TickLabels property. True if the text in the object changes font size when the object size changes. The default value is True
## TickLabels.AutoScaleFont property
True if the text in the object changes font size when the object size changes. The default value is True.
```csharp
public bool AutoScaleFont { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TickLabelsPropertyAutoScaleFontDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Cells cells = sheet.Cells;
// Sample data
cells["A1"].PutValue("Region");
cells["A2"].PutValue("France");
cells["A3"].PutValue("Germany");
cells["A4"].PutValue("England");
cells["B1"].PutValue("Sales");
cells["B2"].PutValue(100000);
cells["B3"].PutValue(150000);
cells["B4"].PutValue(90000);
// Create chart
int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
// Configure chart data
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Configure axis labels with AutoScaleFont
chart.CategoryAxis.TickLabels.AutoScaleFont = true;
chart.CategoryAxis.TickLabels.Font.Size = 12; // Initial size
// Save the workbook
workbook.Save("TickLabelsAutoScaleFontDemo.xlsx");
}
}
}
```
### See Also
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
