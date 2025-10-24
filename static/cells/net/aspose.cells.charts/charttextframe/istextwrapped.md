##ChartTextFrame.IsTextWrapped
ChartTextFrame property. Gets or sets a value indicating whether the text is wrapped
## ChartTextFrame.IsTextWrapped property
Gets or sets a value indicating whether the text is wrapped.
```csharp
public virtual bool IsTextWrapped { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ChartTextFramePropertyIsTextWrappedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("Q1");
sheet.Cells["A3"].PutValue("Q2");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["B2"].PutValue(12000);
sheet.Cells["B3"].PutValue(15000);
// Add chart
int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 20, 10);
Chart chart = sheet.Charts[chartIndex];
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Set chart title with text wrapping
chart.Title.Text = "Quarterly Sales Report (2023) - This is a long title that will wrap when IsTextWrapped is true";
chart.Title.IsTextWrapped = true;
// Save workbook
workbook.Save("ChartTextWrappingDemo.xlsx");
}
}
}
```
### See Also
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
