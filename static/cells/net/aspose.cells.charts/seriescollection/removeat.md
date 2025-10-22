##SeriesCollection.RemoveAt
SeriesCollection method. Remove at a series at the specific index
## SeriesCollection.RemoveAt method
Remove at a series at the specific index.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class SeriesCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Q1");
worksheet.Cells["A3"].PutValue("Q2");
worksheet.Cells["A4"].PutValue("Q3");
worksheet.Cells["B1"].PutValue("Series1");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
worksheet.Cells["C1"].PutValue("Series2");
worksheet.Cells["C2"].PutValue(150);
worksheet.Cells["C3"].PutValue(250);
worksheet.Cells["C4"].PutValue(350);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B1:B4", true);
chart.NSeries.Add("C1:C4", true);
chart.NSeries.CategoryData = "A2:A4";
try
{
// Call RemoveAt to remove the first series (index 0)
chart.NSeries.RemoveAt(0);
Console.WriteLine("Series at index 0 removed successfully");
// Verify the remaining series count
Console.WriteLine($"Remaining series count: {chart.NSeries.Count}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
}
// Save the result
workbook.Save("SeriesCollectionMethodRemoveAtWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
