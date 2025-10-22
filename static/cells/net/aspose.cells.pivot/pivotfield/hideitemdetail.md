##PivotField.HideItemDetail
PivotField method. Sets whether the specific PivotItem in a pivot field is hidden detail
## PivotField.HideItemDetail method
Sets whether the specific PivotItem in a pivot field is hidden detail.
```csharp
public void HideItemDetail(int index, bool isHiddenDetail)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the pivotItem in the pivotField. |
| isHiddenDetail | Boolean | whether the specific PivotItem is hidden |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldMethodHideItemDetailWithInt32BooleanDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("SampleData.xlsx");
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Region");
worksheet.Cells["A2"].PutValue("North");
worksheet.Cells["A3"].PutValue("South");
worksheet.Cells["A4"].PutValue("East");
worksheet.Cells["A5"].PutValue("West");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["B4"].PutValue(3000);
worksheet.Cells["B5"].PutValue(4000);
// Add pivot table
int index = worksheet.PivotTables.Add("A1:B5", "H5", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add fields to areas
pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Get the pivot field
PivotField pivotField = pivotTable.RowFields[0];
// Hide item detail at index 2 (East) with isHidden=false
pivotField.HideItemDetail(2, false);
// Refresh and calculate pivot table data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTable_HideItemDetail_Output.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
