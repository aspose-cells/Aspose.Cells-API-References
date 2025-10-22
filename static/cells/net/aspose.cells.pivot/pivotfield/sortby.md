##PivotField.SortBy
PivotField method. Sorts this pivot field
## SortBy(SortOrder, int) {#sortby}
Sorts this pivot field.
```csharp
public void SortBy(SortOrder sortType, int fieldSortedBy)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sortType | SortOrder | The type of sorting this field. |
| fieldSortedBy | Int32 | The index of pivot field sorted by. -1 means sorting by data labels of this field, others mean the index of data field sorted by. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldMethodSortByWithSortOrderInt32Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Country");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("USA");
worksheet.Cells["A3"].PutValue("UK");
worksheet.Cells["A4"].PutValue("Germany");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["B4"].PutValue(1500);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
PivotField rowField = pivotTable.RowFields[rowIndex];
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Sort the row field in descending order with index -1
rowField.SortBy(SortOrder.Descending, -1);
// Refresh and calculate pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldSortByDemo.xlsx");
}
}
}
```
### See Also
* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## SortBy(SortOrder, int, PivotLineType, string) {#sortby_1}
Sorts this pivot field.
```csharp
public void SortBy(SortOrder sortType, int fieldSortedBy, PivotLineType dataType, string cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sortType | SortOrder | The type of sorting this field. |
| fieldSortedBy | Int32 | The index of pivot field sorted by. -1 means sorting by data labels of this field, others mean the index of data field sorted by. |
| dataType | PivotLineType | The type of data sorted by. |
| cellName | String | Sort by values in the row or column |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldMethodSortByWithSortOrderInt32PivotLineTypeStrDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("B");
worksheet.Cells["A3"].PutValue("A");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B2"].PutValue(200);
worksheet.Cells["B3"].PutValue(300);
worksheet.Cells["B4"].PutValue(100);
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Sort the row field
pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E4");
// Calculate data
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldSortByDemo.xlsx");
}
}
}
```
### See Also
* enum [SortOrder](../../../aspose.cells/sortorder/)
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
