##PivotFilterCollection.Add
PivotFilterCollection method. Adds a PivotFilter Object to the specific type
## PivotFilterCollection.Add method
Adds a PivotFilter Object to the specific type
```csharp
[Obsolete("Use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods,instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int fieldIndex, PivotFilterType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | the PivotField index |
| type | PivotFilterType | the PivotFilter type |
### Return Value
the index of the PivotFilter Object in this PivotFilterCollection.
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterCollectionMethodAddWithInt32PivotFilterTypeDemo
{
public static void Run()
{
Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
// Sample data
cells["A1"].Value = "Category";
cells["A2"].Value = "A";
cells["A3"].Value = "B";
cells["A4"].Value = "A";
cells["A5"].Value = "B";
cells["B1"].Value = "Value";
cells["B2"].Value = 10;
cells["B3"].Value = 20;
cells["B4"].Value = 30;
cells["B5"].Value = 40;
// Create pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int pivotIndex = pivotTables.Add("=A1:B5", "D1", "PivotTable1");
PivotTable pivot = pivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "Category");
pivot.AddFieldToArea(PivotFieldType.Data, "Value");
// Add pivot filter
int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[filterIndex];
filter.AutoFilter.FilterTop10(0, false, false, 2);
pivot.RefreshData();
pivot.CalculateData();
book.Save("PivotFilterDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
