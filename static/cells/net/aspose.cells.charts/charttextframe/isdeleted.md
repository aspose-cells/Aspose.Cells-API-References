##ChartTextFrame.IsDeleted
ChartTextFrame property. Indicates whether this data labels is deleted
## ChartTextFrame.IsDeleted property
Indicates whether this data labels is deleted.
```csharp
public bool IsDeleted { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartTextFramePropertyIsDeletedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
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
// Access data labels and demonstrate IsDeleted property
chart.NSeries[0].DataLabels.ShowValue = true;
bool isDeletedBefore = chart.NSeries[0].DataLabels.IsDeleted;
// Remove data labels by setting ShowValue to false
chart.NSeries[0].DataLabels.ShowValue = false;
bool isDeletedAfter = chart.NSeries[0].DataLabels.IsDeleted;
Console.WriteLine($"DataLabels IsDeleted before removal: {isDeletedBefore}");
Console.WriteLine($"DataLabels IsDeleted after removal: {isDeletedAfter}");
}
}
}
```
### See Also
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
