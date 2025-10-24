##PivotItem.GetFormula
PivotItem method. Gets the formula of this calculated item. Only works when this item is calculated item
## PivotItem.GetFormula method
Gets the formula of this calculated item. Only works when this item is calculated item.
```csharp
public string GetFormula()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemMethodGetFormulaDemo
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
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 150;
worksheet.Cells["B4"].Value = 200;
// Add a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field and data field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Get formula from pivot items
string rowItemFormula = pivotTable.RowFields[0].PivotItems[0].GetFormula();
string dataFieldFormula = pivotTable.DataFields[0].GetFormula();
Console.WriteLine("Row Item Formula: " + rowItemFormula);
Console.WriteLine("Data Field Formula: " + dataFieldFormula);
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
