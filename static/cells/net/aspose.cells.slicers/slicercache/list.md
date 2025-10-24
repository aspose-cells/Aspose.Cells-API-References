##SlicerCache.List
SlicerCache property. Returns whether the slicer associated with the specified slicer cache is based on an NonOLAP data source. Readonly
## SlicerCache.List property
Returns whether the slicer associated with the specified slicer cache is based on an Non-OLAP data source. Read-only
```csharp
public bool List { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class SlicerCachePropertyListDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create sample data
sheet.Cells["A1"].PutValue("Product");
sheet.Cells["A2"].PutValue("Apple");
sheet.Cells["A3"].PutValue("Banana");
sheet.Cells["A4"].PutValue("Cherry");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["B2"].PutValue(100);
sheet.Cells["B3"].PutValue(200);
sheet.Cells["B4"].PutValue(300);
// Create table with correct overload
int tableIdx = sheet.ListObjects.Add(0, 0, 3, 1, true);
Aspose.Cells.Tables.ListObject table = sheet.ListObjects[tableIdx];
table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;
// Add slicer
int slicerIdx = sheet.Slicers.Add(table, 0, "D2");
Slicer slicer = sheet.Slicers[slicerIdx];
// Access slicer cache
SlicerCache cache = slicer.SlicerCache;
// Demonstrate List property usage
Console.WriteLine("Slicer uses Non-OLAP data source: " + cache.List);
}
}
}
```
### See Also
* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
