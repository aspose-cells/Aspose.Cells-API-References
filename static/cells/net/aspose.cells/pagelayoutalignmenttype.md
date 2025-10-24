##Enum PageLayoutAlignmentType
Aspose.Cells.PageLayoutAlignmentType enum. Enumerates page layout alignment types
## PageLayoutAlignmentType enumeration
Enumerates page layout alignment types.
```csharp
public enum PageLayoutAlignmentType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Bottom | `0` | Represents bottom page layout alignment. |
| Center | `1` | Represents center page layout alignment. |
| Left | `2` | Represents left page layout alignment. |
| Right | `3` | Represents right page layout alignment. |
| Top | `4` | Represents top page layout alignment. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class PageLayoutAlignmentTypeDemo
{
public static void PageLayoutAlignmentTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to the worksheet
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["A2"].PutValue(123);
worksheet.Cells["A3"].PutValue(456);
worksheet.Cells["A4"].PutValue(789);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set the data range for the chart
chart.SetChartDataRange("A1:A4", true);
// Set the title of the chart
chart.Title.Text = "Sample Chart";
// Save the workbook to a file
workbook.Save("PageLayoutAlignmentTypeExample.xlsx");
// Export the chart to a PDF with specific page layout alignment
chart.ToPdf("ChartExample.pdf", 8.5f, 11f, PageLayoutAlignmentType.Center, PageLayoutAlignmentType.Center);
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
