##PivotField.FilterTop10
PivotField method. Filters by values of data pivot field
## PivotField.FilterTop10 method
Filters by values of data pivot field.
```csharp
public PivotFilter FilterTop10(int valueFieldIndex, PivotFilterType type, bool isTop, int itemCount)
```
| Parameter | Type | Description |
| --- | --- | --- |
| valueFieldIndex | Int32 | The index of data field in the data region. |
| type | PivotFilterType | The type of filtering data. Only can be Count,Sum and Percent. |
| isTop | Boolean | Indicates whether filter from top or bottom |
| itemCount | Int32 | The item count |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldMethodFilterTop10WithInt32PivotFilterTypeBooleanIntDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["A5"].Value = "Apple";
worksheet.Cells["A6"].Value = "Orange";
worksheet.Cells["A7"].Value = "Banana";
worksheet.Cells["A8"].Value = "Apple";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 20;
worksheet.Cells["B4"].Value = 30;
worksheet.Cells["B5"].Value = 40;
worksheet.Cells["B6"].Value = 50;
worksheet.Cells["B7"].Value = 60;
worksheet.Cells["B8"].Value = 70;
// Create pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:B8", "C3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Apply top 10 filter
pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
// Save the workbook
workbook.Save("PivotTableFilterTop10.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
