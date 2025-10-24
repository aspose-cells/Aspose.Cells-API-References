##DataLabels.NumberFormatLinked
DataLabels property. True if the number format is linked to the cells so that the number format changes in the labels when it changes in the cells
## DataLabels.NumberFormatLinked property
True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).
```csharp
public bool NumberFormatLinked { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyNumberFormatLinkedDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["C1"].PutValue("Formatted Value");
worksheet.Cells["C2"].PutValue("100 units");
worksheet.Cells["C3"].PutValue("200 units");
// Create a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Add series
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Configure data labels
var series = chart.NSeries[0];
series.DataLabels.ShowValue = true;
series.DataLabels.LinkedSource = "C2:C3";
series.DataLabels.NumberFormatLinked = true; // Link number format from source cells
// Save the workbook
workbook.Save("DataLabelsNumberFormatLinkedDemo.xlsx");
}
}
}
```
### See Also
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
