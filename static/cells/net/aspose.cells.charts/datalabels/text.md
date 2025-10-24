##DataLabels.Text
DataLabels property. Gets or sets the text of data label
## DataLabels.Text property
Gets or sets the text of data label.
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
public class DataLabelsPropertyTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Product A");
worksheet.Cells["A3"].PutValue("Product B");
worksheet.Cells["A4"].PutValue("Product C");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Enable data labels
for (int i = 0; i < chart.NSeries.Count; i++)
{
Aspose.Cells.Charts.Series series = chart.NSeries[i];
series.DataLabels.ShowValue = true;
// Customize data label text
for (int j = 0; j < series.Points.Count; j++)
{
series.Points[j].DataLabels.Text = $"+{series.Points[j].YValue}";
}
}
// Save the workbook
workbook.Save("DataLabelsTextDemo.xlsx");
}
}
}
```
### See Also
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
