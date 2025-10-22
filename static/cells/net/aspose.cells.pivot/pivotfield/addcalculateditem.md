##PivotField.AddCalculatedItem
PivotField method. Add a calculated formula item to the pivot field
## PivotField.AddCalculatedItem method
Add a calculated formula item to the pivot field.
```csharp
public void AddCalculatedItem(string name, string formula)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The item's name. |
| formula | String | The formula of pivot item. |
### Remarks
Only supports to add calculated item to Row/Column field.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldMethodAddCalculatedItemWithStringStringDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].Value = "Fruit";
sheet.Cells["A2"].Value = "grape";
sheet.Cells["A3"].Value = "kiwi";
sheet.Cells["A4"].Value = "grape";
sheet.Cells["A5"].Value = "kiwi";
sheet.Cells["B1"].Value = "Sales";
sheet.Cells["B2"].Value = 50;
sheet.Cells["B3"].Value = 70;
sheet.Cells["B4"].Value = 30;
sheet.Cells["B5"].Value = 20;
// Create pivot table with correct parameters
int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Get the pivot field and add calculated item
PivotField fruitField = pivotTable.RowFields[0];
fruitField.AddCalculatedItem("grape_kiwi_total", "=grape + kiwi");
// Refresh and calculate pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldAddCalculatedItemDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
