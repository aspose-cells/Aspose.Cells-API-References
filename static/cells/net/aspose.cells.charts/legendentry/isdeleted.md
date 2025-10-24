##LegendEntry.IsDeleted
LegendEntry property. Gets and sets whether the legend entry is deleted
## LegendEntry.IsDeleted property
Gets and sets whether the legend entry is deleted.
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
public class LegendEntryPropertyIsDeletedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Product A");
worksheet.Cells["A3"].PutValue("Product B");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Get the first legend entry
LegendEntry legendEntry = chart.Legend.LegendEntries[0];
// Demonstrate IsDeleted property
Console.WriteLine("Legend entry initially deleted? " + legendEntry.IsDeleted);
// Delete the legend entry
legendEntry.IsDeleted = true;
Console.WriteLine("Legend entry after deletion? " + legendEntry.IsDeleted);
// Restore the legend entry
legendEntry.IsDeleted = false;
Console.WriteLine("Legend entry after restoration? " + legendEntry.IsDeleted);
// Save the workbook
workbook.Save("LegendEntryIsDeletedDemo.xlsx");
}
}
}
```
### See Also
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
