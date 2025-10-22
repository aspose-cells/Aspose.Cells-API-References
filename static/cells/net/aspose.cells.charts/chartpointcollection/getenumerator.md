##ChartPointCollection.GetEnumerator
ChartPointCollection method. Returns an enumerator for the entire ChartPointCollection
## ChartPointCollection.GetEnumerator method
Returns an enumerator for the entire [`ChartPointCollection`](../).
```csharp
public IEnumerator GetEnumerator()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Collections;
public class ChartPointCollectionMethodGetEnumeratorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Cat1");
worksheet.Cells["A3"].PutValue("Cat2");
worksheet.Cells["A4"].PutValue("Cat3");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
try
{
// Get the first series' points collection
ChartPointCollection points = chart.NSeries[0].Points;
// Call the GetEnumerator method
IEnumerator enumerator = points.GetEnumerator();
Console.WriteLine("Iterating through chart points:");
while (enumerator.MoveNext())
{
ChartPoint point = (ChartPoint)enumerator.Current;
Console.WriteLine($"Point value: {point.YValue}");
}
Console.WriteLine("Method executed successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetEnumeratorDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
