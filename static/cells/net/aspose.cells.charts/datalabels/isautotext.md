##DataLabels.IsAutoText
DataLabels property. Indicates the text is auto generated
## DataLabels.IsAutoText property
Indicates the text is auto generated.
```csharp
public override bool IsAutoText { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyIsAutoTextDemo
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
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Enable data labels
foreach (Series series in chart.NSeries)
{
series.DataLabels.ShowValue = true;
// Demonstrate IsAutoText property
foreach (ChartPoint point in series.Points)
{
Console.WriteLine("IsAutoText before setting: " + point.DataLabels.IsAutoText);
point.DataLabels.IsAutoText = false;
point.DataLabels.Text = "Custom " + point.YValue;
Console.WriteLine("IsAutoText after setting: " + point.DataLabels.IsAutoText);
Console.WriteLine("DataLabel Text: " + point.DataLabels.Text);
}
}
// Save the workbook
workbook.Save("DataLabelsIsAutoTextDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
