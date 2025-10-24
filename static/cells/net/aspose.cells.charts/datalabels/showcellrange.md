##DataLabels.ShowCellRange
DataLabels property. Indicates whether showing cell range as the data labels
## DataLabels.ShowCellRange property
Indicates whether showing cell range as the data labels.
```csharp
public bool ShowCellRange { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyShowCellRangeDemo
{
public static void Run()
{
// Create workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["C2"].PutValue("100 units");
worksheet.Cells["C3"].PutValue("200 units");
// Create chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Configure data labels with ShowCellRange
var series = chart.NSeries[0];
series.DataLabels.ShowValue = true;
series.DataLabels.ShowCellRange = true;
series.DataLabels.LinkedSource = "C2:C3";
series.DataLabels.Font.Color = Color.Blue;
// Save the workbook
workbook.Save("DataLabelsShowCellRangeDemo.xlsx");
}
}
}
```
### See Also
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
