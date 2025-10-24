##SlicerCache.CrossFilterType
SlicerCache property. Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache and how cross filtering is displayed. Read/write
## SlicerCache.CrossFilterType property
Returns or sets whether a slicer is participating in cross filtering with other slicers that share the same slicer cache, and how cross filtering is displayed. Read/write
```csharp
public SlicerCacheCrossFilterType CrossFilterType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicerCachePropertyCrossFilterTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Add slicer
int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "Category");
Slicer slicer = worksheet.Slicers[slicerIndex];
// Set and demonstrate CrossFilterType
slicer.SlicerCache.CrossFilterType = SlicerCacheCrossFilterType.ShowItemsWithDataAtTop;
Console.WriteLine("Slicer CrossFilterType: " + slicer.SlicerCache.CrossFilterType);
workbook.Save("SlicerCacheCrossFilterTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [SlicerCacheCrossFilterType](../../slicercachecrossfiltertype/)
* class [SlicerCache](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
