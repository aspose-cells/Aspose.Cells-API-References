##PivotFilterCollection.AddValueFilter
PivotFilterCollection method. Filters by values of data pivot field
## PivotFilterCollection.AddValueFilter method
Filters by values of data pivot field.
```csharp
public PivotFilter AddValueFilter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type,
double value1, double value2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | The index of field in the source. |
| valueFieldIndex | Int32 | The index of value field in the value region. |
| type | PivotFilterType | The type of filtering data. |
| value1 | Double | The value of filter condition |
| value2 | Double | The upper-bound value of between filter condition |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFilterCollectionMethodAddValueFilterWithInt32Int32PivotFilterTypeDoublDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["A2"].Value = "Widget";
worksheet.Cells["A3"].Value = "Gadget";
worksheet.Cells["A4"].Value = "Thingy";
worksheet.Cells["B1"].Value = "Price";
worksheet.Cells["B2"].Value = 15.99;
worksheet.Cells["B3"].Value = 24.99;
worksheet.Cells["B4"].Value = 9.99;
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
// Add value filter to show products priced between $10 and $20
PivotFilter filter = filters.AddValueFilter(
baseFieldIndex: 0,
valueFieldIndex: 1,
type: PivotFilterType.ValueBetween,
value1: 10.0,
value2: 20.0
);
Console.WriteLine($"Value filter added successfully. Filter type: {filter.FilterType}");
Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
}
catch (Exception ex)
{
Console.WriteLine($"Error adding value filter: {ex.Message}");
}
workbook.Save("PivotFilterCollectionMethodAddValueFilterDemo.xlsx");
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
