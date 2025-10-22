##PivotTableCollection.Remove
PivotTableCollection method. Deletes the specified PivotTable and delete the PivotTable data
## Remove(PivotTable) {#remove}
Deletes the specified PivotTable and delete the PivotTable data
```csharp
public void Remove(PivotTable pivotTable)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable object |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableCollectionMethodRemoveWithPivotTableDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("PivotTableExample.xlsx");
// Access first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Get pivot table collection
PivotTableCollection pivotTables = sheet.PivotTables;
// Check if there are any pivot tables
if (pivotTables.Count > 0)
{
// Get first pivot table
PivotTable pivotTable = pivotTables[0];
// Remove the pivot table
pivotTables.Remove(pivotTable);
Console.WriteLine("Pivot table removed successfully. Count: " + pivotTables.Count);
}
// Save the workbook
workbook.Save("PivotTableRemoved.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## Remove(PivotTable, bool) {#remove_1}
Deletes the specified PivotTable
```csharp
public void Remove(PivotTable pivotTable, bool keepData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | PivotTable object |
| keepData | Boolean | Whether to keep the PivotTable data |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableCollectionMethodRemoveWithPivotTableBooleanDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
// Add a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "D5", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
pivotTable.RefreshData();
pivotTable.CalculateData();
// Demonstrate Remove method with PivotTable and boolean parameters
Console.WriteLine("Before removal - Cell D5 value: " + worksheet.Cells["D5"].StringValue);
// Remove pivot table but keep the data (true)
worksheet.PivotTables.Remove(pivotTable, true);
Console.WriteLine("After removal (keep data) - Cell D5 value: " + worksheet.Cells["D5"].StringValue);
// Add another pivot table
index = worksheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
pivotTable.RefreshData();
pivotTable.CalculateData();
Console.WriteLine("\nBefore removal - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
// Remove pivot table and clear data (false)
worksheet.PivotTables.Remove(pivotTable, false);
Console.WriteLine("After removal (clear data) - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
}
}
}
```
### See Also
* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
