##Enum SlicerCacheCrossFilterType
Aspose.Cells.Slicers.SlicerCacheCrossFilterType enum. Represent the type of SlicerCacheCrossFilterType
## SlicerCacheCrossFilterType enumeration
Represent the type of SlicerCacheCrossFilterType
```csharp
public enum SlicerCacheCrossFilterType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | The table style element of the slicer style for slicer items with no data is not applied to slicer items with no data, and slicer items with no data are not sorted separately in the list of slicer items in the slicer view |
| ShowItemsWithDataAtTop | `1` | The table style element of the slicer style for slicer items with no data is applied to slicer items with no data, and slicer items with no data are sorted at the bottom in the list of slicer items in the slicer view |
| ShowItemsWithNoData | `2` | The table style element of the slicer style for slicer items with no data is applied to slicer items with no data, and slicer items with no data are not sorted separately in the list of slicer items in the slicer view. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;
using System;
public class SlicerCacheCrossFilterTypeDemo
{
public static void SlicerCacheCrossFilterTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a pivot table to the worksheet
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Add a slicer to the worksheet
int slicerIndex = worksheet.Slicers.Add(pivotTable, "C10", "Category");
Slicer slicer = worksheet.Slicers[slicerIndex];
// Set the cross filter type for the slicer cache
slicer.SlicerCache.CrossFilterType = SlicerCacheCrossFilterType.ShowItemsWithDataAtTop;
worksheet.Cells["A3"].PutValue("");
worksheet.RefreshPivotTables();
// Output the cross filter type
Console.WriteLine("Slicer Cache Cross Filter Type: " + slicer.SlicerCache.CrossFilterType);
// Save the workbook
workbook.Save("SlicerCacheCrossFilterTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)
