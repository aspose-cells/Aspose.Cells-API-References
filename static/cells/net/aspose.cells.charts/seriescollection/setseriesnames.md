##SeriesCollection.SetSeriesNames
SeriesCollection method. Sets the name of all the serieses in the chart
## SeriesCollection.SetSeriesNames method
Sets the name of all the serieses in the chart.
```csharp
public void SetSeriesNames(int startIndex, string area, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | The index of the first series which you want to set the name. |
| area | String | Specifies the area for the series name. |
| isVertical | Boolean | &gt;Specifies whether to plot the series from a range of cell values by row or by column. |
### Remarks
If the start index is larger than the count of the serieses, it will return and do nothing.If set data on contiguous cells, use colon to seperate them.For example, $C$2:$C$5.If set data on contiguous cells, use comma to seperate them.For example, ($C$2,$D$5).
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Q1");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(150);
worksheet.Cells["B4"].PutValue(200);
worksheet.Cells["C1"].PutValue("Q2");
worksheet.Cells["C2"].PutValue(120);
worksheet.Cells["C3"].PutValue(180);
worksheet.Cells["C4"].PutValue(220);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Get the chart's series collection
SeriesCollection seriesCollection = chart.NSeries;
try
{
// Call SetSeriesNames with parameters (startIndex: 0, area: "A2:A4", isVertical: true)
seriesCollection.SetSeriesNames(0, "A2:A4", true);
// Add series data
seriesCollection.Add("B2:C4", true);
Console.WriteLine("SetSeriesNames method executed successfully with parameters (Int32, String, Boolean)");
Console.WriteLine("Series names set from range A2:A4");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetSeriesNames method: {ex.Message}");
}
// Save the result
workbook.Save("SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo.xlsx");
}
}
}
```
### See Also
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
