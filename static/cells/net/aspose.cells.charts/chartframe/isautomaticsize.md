##ChartFrame.IsAutomaticSize
ChartFrame property. Indicates whether the chart frame is automatic sized
## ChartFrame.IsAutomaticSize property
Indicates whether the chart frame is automatic sized.
```csharp
public virtual bool IsAutomaticSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartFramePropertyIsAutomaticSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access legend and demonstrate IsAutomaticSize property
Aspose.Cells.Charts.Legend legend = chart.Legend;
// Set automatic size to false and show the value
legend.IsAutomaticSize = false;
Console.WriteLine("Legend Automatic Size: " + legend.IsAutomaticSize);
// Set automatic size to true and show the value
legend.IsAutomaticSize = true;
Console.WriteLine("Legend Automatic Size: " + legend.IsAutomaticSize);
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
