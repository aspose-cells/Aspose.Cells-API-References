##LegendEntryCollection.Item
LegendEntryCollection property. Gets the LegendEntry element at the specified index
## LegendEntryCollection indexer
Gets the [`LegendEntry`](../../legendentry/) element at the specified index.
```csharp
public LegendEntry this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class LegendEntryCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category 1");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
worksheet.Cells["B1"].PutValue("Category 2");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["B3"].PutValue(40);
// Create a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("A2:B3", true);
chart.NSeries.CategoryData = "A1:B1";
// Access legend entries
LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
// Demonstrate Item property usage
for (int i = 0; i < legendEntries.Count; i++)
{
LegendEntry entry = legendEntries[i];
Console.WriteLine($"Legend Entry {i}:");
Console.WriteLine($"- Font: {entry.Font.Name}");
Console.WriteLine($"- Auto Scale Font: {entry.AutoScaleFont}");
}
// Modify first legend entry
if (legendEntries.Count > 0)
{
legendEntries[0].Font.Name = "Arial";
legendEntries[0].Font.Size = 12;
legendEntries[0].AutoScaleFont = false;
}
}
}
}
```
### See Also
* class [LegendEntry](../../legendentry/)
* class [LegendEntryCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
