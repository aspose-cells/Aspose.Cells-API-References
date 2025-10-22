##Enum PrintSizeType
Aspose.Cells.PrintSizeType enum. Represents the printed chart size
## PrintSizeType enumeration
Represents the printed chart size.
```csharp
public enum PrintSizeType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Full | `0` | Use full page. |
| Fit | `1` | Scale to fit page. |
| Custom | `2` | Custom. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class PrintSizeTypeDemo
{
public static void PrintSizeTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells[0, 0].PutValue("Category");
worksheet.Cells[0, 1].PutValue("Value");
worksheet.Cells[1, 0].PutValue("A");
worksheet.Cells[1, 1].PutValue(10);
worksheet.Cells[2, 0].PutValue("B");
worksheet.Cells[2, 1].PutValue(20);
worksheet.Cells[3, 0].PutValue("C");
worksheet.Cells[3, 1].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set the data range for the chart
chart.SetChartDataRange("A1:B4", true);
// Set the chart title
chart.Title.Text = "Sample Chart";
// Set the print size of the chart
chart.PrintSize = PrintSizeType.Fit;
// Save the workbook
workbook.Save("PrintSizeTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
