##SlicerCacheItemCollection.Item
SlicerCacheItemCollection property. Gets the SlicerCacheItem object by index
## SlicerCacheItemCollection indexer
Gets the SlicerCacheItem object by index.
```csharp
public SlicerCacheItem this[int index] { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicerCacheItemCollectionPropertyItemDemo
{
public static void Run()
{
// Create a workbook and add a pivot table
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].Value = "Fruit";
sheet.Cells["A2"].Value = "Apple";
sheet.Cells["A3"].Value = "Orange";
sheet.Cells["A4"].Value = "Banana";
sheet.Cells["B1"].Value = "Sales";
sheet.Cells["B2"].Value = 100;
sheet.Cells["B3"].Value = 200;
sheet.Cells["B4"].Value = 300;
// Create pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotIndex];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Add slicer
SlicerCollection slicers = sheet.Slicers;
int slicerIndex = slicers.Add(pivotTable, "Fruit", "A1");
Slicer slicer = slicers[slicerIndex];
// Access slicer cache items using Item property
SlicerCacheItemCollection items = slicer.SlicerCache.SlicerCacheItems;
if (items.Count > 0)
{
SlicerCacheItem item = items[0]; // Demonstrating Item property usage
Console.WriteLine("First slicer item: " + item.Value);
}
}
}
}
```
### See Also
* class [SlicerCacheItem](../../slicercacheitem/)
* class [SlicerCacheItemCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
