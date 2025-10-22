##PivotFilterCollection.AddDateFilter
PivotFilterCollection method. Filters by date setting of row or column pivot field
## PivotFilterCollection.AddDateFilter method
Filters by date setting of row or column pivot field.
```csharp
public PivotFilter AddDateFilter(int baseFieldIndex, PivotFilterType type, DateTime dateTime1,
DateTime dateTime2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | The index of field in the source. |
| type | PivotFilterType | The type of filtering data. |
| dateTime1 | DateTime | The date label of filter condition |
| dateTime2 | DateTime | The upper-bound date label of between filter condition |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFilterCollectionMethodAddDateFilterWithInt32PivotFilterTypeDateTimeDaDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data with dates
worksheet.Cells["A1"].Value = "Date";
worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 1000;
worksheet.Cells["B3"].Value = 2000;
worksheet.Cells["B4"].Value = 3000;
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
// Add date filter to show dates between Jan 1 and Mar 31, 2023
PivotFilter filter = filters.AddDateFilter(
baseFieldIndex: 0,
type: PivotFilterType.DateBetween,
dateTime1: new DateTime(2023, 1, 1),
dateTime2: new DateTime(2023, 3, 31)
);
Console.WriteLine($"Date filter added successfully. Filter type: {filter.FilterType}");
Console.WriteLine($"Field index: {filter.FieldIndex}, UseWholeDay: {filter.UseWholeDay}");
}
catch (Exception ex)
{
Console.WriteLine($"Error adding date filter: {ex.Message}");
}
workbook.Save("PivotFilterCollectionMethodAddDateFilterDemo.xlsx");
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
