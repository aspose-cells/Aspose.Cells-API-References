##Title.Text
Title property. Gets or sets the text of display unit label
## Title.Text property
Gets or sets the text of display unit label.
```csharp
public override string Text { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TitlePropertyTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet and add sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Q1");
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(200);
worksheet.Cells["A4"].PutValue(300);
// Add a chart and set its ValueAxis title text
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.ValueAxis.Title.Text = "Sales Amount";
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
