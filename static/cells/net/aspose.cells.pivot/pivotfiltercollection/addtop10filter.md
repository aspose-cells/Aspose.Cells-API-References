##PivotFilterCollection.AddTop10Filter
PivotFilterCollection method. Filters by values of data pivot field
## PivotFilterCollection.AddTop10Filter method
Filters by values of data pivot field.
```csharp
public PivotFilter AddTop10Filter(int baseFieldIndex, int valueFieldIndex, PivotFilterType type,
bool isTop, int itemCount)
```
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | The index of field in the source. |
| valueFieldIndex | Int32 | The index of data field in the data region. |
| type | PivotFilterType | The type of filtering data. Only can be Count,Sum and Percent. |
| isTop | Boolean | Indicates whether filter from top or bottom |
| itemCount | Int32 | The item count |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFilterCollectionMethodAddTop10FilterWithInt32Int32PivotFilterTypeBooleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["A2"].Value = "Fruit";
worksheet.Cells["A3"].Value = "Vegetable";
worksheet.Cells["A4"].Value = "Dairy";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 150;
worksheet.Cells["B3"].Value = 80;
worksheet.Cells["B4"].Value = 120;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
try
{
// Get pivot filters collection
PivotFilterCollection filters = pivotTable.PivotFilters;
// Add Top10 filter - show top 2 items by sales
PivotFilter filter = filters.AddTop10Filter(
baseFieldIndex: 0,          // Category field
valueFieldIndex: 1,          // Sales field
type: PivotFilterType.Count, // Filter type
isTop: true,                 // Show top items
itemCount: 2                 // Number of items to show
);
Console.WriteLine($"Top10 filter added successfully. Filter type: {filter.FilterType}");
Console.WriteLine($"Field index: {filter.FieldIndex}, Value field index: {filter.ValueFieldIndex}");
}
catch (Exception ex)
{
Console.WriteLine($"Error adding Top10 filter: {ex.Message}");
}
// Save the workbook
workbook.Save("PivotFilterCollectionMethodAddTop10FilterDemo.xlsx");
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
