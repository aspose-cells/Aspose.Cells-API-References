##TickLabels.DisplayNumberFormat
TickLabels property. Gets and sets the display number format of tick labels
## TickLabels.DisplayNumberFormat property
Gets and sets the display number format of tick labels.
```csharp
public string DisplayNumberFormat { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TickLabelsPropertyDisplayNumberFormatDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["A2"].PutValue(DateTime.Now);
worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("A2:A3", true);
chart.NSeries.CategoryData = "B2:B3";
// Set number format through NumberFormat property instead
chart.CategoryAxis.TickLabels.NumberFormat = "m/d/yyyy";
chart.ValueAxis.TickLabels.NumberFormat = "#,##0";
// Save the workbook
workbook.Save("TickLabelsDisplayNumberFormatDemo.xlsx");
Console.WriteLine("DisplayNumberFormat for CategoryAxis: " +
chart.CategoryAxis.TickLabels.DisplayNumberFormat);
Console.WriteLine("DisplayNumberFormat for ValueAxis: " +
chart.ValueAxis.TickLabels.DisplayNumberFormat);
}
}
}
```
### See Also
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
