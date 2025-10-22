##PivotField.ShowValuesAs
PivotField method. Shows values of data field as different display format when the ShowDataAs calculation is in use
## PivotField.ShowValuesAs method
Shows values of data field as different display format when the ShowDataAs calculation is in use.
```csharp
public void ShowValuesAs(PivotFieldDataDisplayFormat displayFormat, int baseField,
PivotItemPositionType baseItemPositionType, int baseItem)
```
| Parameter | Type | Description |
| --- | --- | --- |
| displayFormat | PivotFieldDataDisplayFormat | The data display format type. |
| baseField | Int32 | The index to the field which ShowDataAs calculation bases on. |
| baseItemPositionType | PivotItemPositionType | The position type of base iteam. |
| baseItem | Int32 | The index to the base item which ShowDataAs calculation bases on. Only works when baseItemPositionType is custom. |
### Remarks
Only for data field.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldMethodShowValuesAsWithPivotFieldDataDisplayFormatIntDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[workbook.Worksheets.Add()];
worksheet.Name = "PivotData";
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Quarter");
worksheet.Cells["C1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Electronics");
worksheet.Cells["B2"].PutValue("Q1");
worksheet.Cells["C2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Electronics");
worksheet.Cells["B3"].PutValue("Q2");
worksheet.Cells["C3"].PutValue(1500);
worksheet.Cells["A4"].PutValue("Furniture");
worksheet.Cells["B4"].PutValue("Q1");
worksheet.Cells["C4"].PutValue(800);
worksheet.Cells["A5"].PutValue("Furniture");
worksheet.Cells["B5"].PutValue("Q2");
worksheet.Cells["C5"].PutValue(1200);
// Create pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotIndex = pivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotIndex];
// Add row field
int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
PivotField rowField = pivotTable.RowFields[rowFieldIndex];
// Add column field
int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, "Quarter");
PivotField columnField = pivotTable.ColumnFields[columnFieldIndex];
// Add data field and configure ShowValuesAs
int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
PivotField dataField = pivotTable.DataFields[dataFieldIndex];
dataField.DisplayName = "Sales Diff";
dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, columnField.BaseIndex, PivotItemPositionType.Next, 0);
// Calculate data and save
pivotTable.CalculateData();
workbook.Save("PivotTableShowValuesAsDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* enum [PivotItemPositionType](../../pivotitempositiontype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
