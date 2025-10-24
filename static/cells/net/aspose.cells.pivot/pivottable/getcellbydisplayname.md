##PivotTable.GetCellByDisplayName
PivotTable method. Gets the Cell object by the display name of PivotField
## PivotTable.GetCellByDisplayName method
Gets the [`Cell`](../../../aspose.cells/cell/) object by the display name of PivotField.
```csharp
public Cell GetCellByDisplayName(string displayName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| displayName | String | the DisplayName of PivotField |
### Return Value
the Cell object
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodGetCellByDisplayNameWithStringDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 15;
cells["A4"].Value = "Banana";
cells["B4"].Value = 20;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field and data field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Refresh and calculate pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Get data field display name
string displayName = pivotTable.DataFields[0].DisplayName;
// Use GetCellByDisplayName method
Cell cell = pivotTable.GetCellByDisplayName(displayName);
// Output results
Console.WriteLine("Display Name: " + displayName);
Console.WriteLine("Cell Name: " + (cell != null ? cell.Name : "null"));
Console.WriteLine("Cell Value: " + (cell != null ? cell.Value.ToString() : "null"));
// Save the workbook
workbook.Save("PivotTable_GetCellByDisplayName_Output.xlsx");
}
}
}
```
### See Also
* class [Cell](../../../aspose.cells/cell/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
