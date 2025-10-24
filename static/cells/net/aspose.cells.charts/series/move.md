##Series.Move
Series method. Moves the series up or down
## Series.Move method
Moves the series up or down.
```csharp
public void Move(int count)
```
| Parameter | Type | Description |
| --- | --- | --- |
| count | Int32 | The number of moving up or down. Move the series up if this is less than zero; Move the series down if this is greater than zero. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class SeriesMethodMoveWithInt32Demo
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
// Add series to the chart
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the first series
Series series = chart.NSeries[0];
try
{
// Call the Move method with Int32 parameter
series.Move(1);
Console.WriteLine("Series moved successfully by 1 position");
// Show effect by changing series name
series.Name = "Moved Series";
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Move method: {ex.Message}");
}
// Save the result
workbook.Save("SeriesMethodMoveWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
