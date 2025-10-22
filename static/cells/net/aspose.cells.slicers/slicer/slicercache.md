##Slicer.SlicerCache
Slicer property. Returns the SlicerCache object associated with the slicer. Readonly
## Slicer.SlicerCache property
Returns the SlicerCache object associated with the slicer. Read-only.
```csharp
public SlicerCache SlicerCache { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicerPropertySlicerCacheDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Fruit");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(15);
worksheet.Cells["B4"].PutValue(20);
// Create a table from the data range
int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
// Add a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Add a slicer
int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "Slicer1");
Slicer slicer = worksheet.Slicers[slicerIndex];
// Demonstrate SlicerCache usage
SlicerCache slicerCache = slicer.SlicerCache;
Console.WriteLine("Slicer Cache Name: " + slicerCache.Name);
Console.WriteLine("Slicer Cache Source Name: " + slicerCache.SourceName);
Console.WriteLine("Slicer Cache Items Count: " + slicerCache.SlicerCacheItems.Count);
// Save the workbook
workbook.Save("SlicerCacheDemo.xlsx");
}
}
}
```
### See Also
* class [SlicerCache](../../slicercache/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
