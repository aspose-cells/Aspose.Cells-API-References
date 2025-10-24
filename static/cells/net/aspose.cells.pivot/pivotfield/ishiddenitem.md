##PivotField.IsHiddenItem
PivotField method. Gets whether the specific PivotItem is hidden
## PivotField.IsHiddenItem method
Gets whether the specific PivotItem is hidden.
```csharp
public bool IsHiddenItem(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the pivotItem in the pivotField. |
### Return Value
whether the specific PivotItem is hidden
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldMethodIsHiddenItemWithInt32Demo
{
public static void Run()
{
// Create a workbook and add sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Country";
worksheet.Cells["A2"].Value = "USA";
worksheet.Cells["A3"].Value = "Canada";
worksheet.Cells["A4"].Value = "UK";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 1000;
worksheet.Cells["B3"].Value = 2000;
worksheet.Cells["B4"].Value = 3000;
// Create pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
PivotField rowField = pivotTable.RowFields[0];
// Hide item at index 1 (Canada)
rowField.HideItem(1, true);
pivotTable.RefreshData();
pivotTable.CalculateData();
// Check if item at index 1 is hidden
bool isHidden = rowField.IsHiddenItem(1);
Console.WriteLine("Is item at index 1 hidden? " + isHidden);
// Save the workbook
workbook.Save("PivotFieldIsHiddenItemDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
