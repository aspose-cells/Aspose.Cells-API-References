##ChartCollection.RemoveAt
ChartCollection method. Remove a chart at the specific index
## ChartCollection.RemoveAt method
Remove a chart at the specific index.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The chart index. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for the chart
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["A3"].PutValue("B");
sheet.Cells["B3"].PutValue(20);
// Add a chart to the worksheet
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Display initial chart count
Console.WriteLine("Initial chart count: " + sheet.Charts.Count);
// Remove the chart at index 0
sheet.Charts.RemoveAt(0);
// Display chart count after removal
Console.WriteLine("Chart count after removal: " + sheet.Charts.Count);
}
}
}
```
### See Also
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
