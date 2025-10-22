##Legend.LegendEntries
Legend property. Gets a collection of all the LegendEntry objects in the specified chart legend. Setting the legend entries of the surface chart is not supported. So it will return null if the chart type is surface chart type
## Legend.LegendEntries property
Gets a collection of all the LegendEntry objects in the specified chart legend. Setting the legend entries of the surface chart is not supported. So it will return null if the chart type is surface chart type.
```csharp
public LegendEntryCollection LegendEntries { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class LegendPropertyLegendEntriesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
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
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("A2:A4", true);
chart.NSeries.CategoryData = "B2:B4";
// Access legend entries
Aspose.Cells.Charts.LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
// Delete the second legend entry
legendEntries[1].IsDeleted = true;
// Save the workbook
workbook.Save("LegendEntriesDemo.xlsx");
}
}
}
```
### See Also
* class [LegendEntryCollection](../../legendentrycollection/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
