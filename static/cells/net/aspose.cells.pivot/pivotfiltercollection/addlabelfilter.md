##PivotFilterCollection.AddLabelFilter
PivotFilterCollection method. Filters by captions of row or column pivot field
## PivotFilterCollection.AddLabelFilter method
Filters by captions of row or column pivot field.
```csharp
public PivotFilter AddLabelFilter(int baseFieldIndex, PivotFilterType type, string label1,
string label2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | The index of field in the source. |
| type | PivotFilterType | The type of filtering data. |
| label1 | String | The label of filter condition |
| label2 | String | The upper-bound label of between filter condition |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFilterCollectionMethodAddLabelFilterWithInt32PivotFilterTypeStringStriDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Banana";
worksheet.Cells["A4"].Value = "Cherry";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 200;
worksheet.Cells["B4"].Value = 300;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
try
{
PivotFilterCollection filters = pivotTable.PivotFilters;
// Add label filter to show products beginning with "A"
PivotFilter filter = filters.AddLabelFilter(
baseFieldIndex: 0,
type: PivotFilterType.CaptionBeginsWith,
label1: "A",
label2: null
);
Console.WriteLine($"Label filter added successfully. Filter type: {filter.FilterType}");
Console.WriteLine($"Field index: {filter.FieldIndex}, Value1: {filter.Value1}");
}
catch (Exception ex)
{
Console.WriteLine($"Error adding label filter: {ex.Message}");
}
workbook.Save("PivotFilterCollectionMethodAddLabelFilterDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
