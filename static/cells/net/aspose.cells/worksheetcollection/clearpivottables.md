##WorksheetCollection.ClearPivottables
WorksheetCollection method. Clears pivot tables from the spreadsheet
## WorksheetCollection.ClearPivottables method
Clears pivot tables from the spreadsheet.
```csharp
public void ClearPivottables()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodClearPivottablesDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(300);
// Add a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
Console.WriteLine("Pivot tables count before clearing: " + worksheet.PivotTables.Count);
// Clear all pivot tables from all worksheets
workbook.Worksheets.ClearPivottables();
Console.WriteLine("Pivot tables count after clearing: " + worksheet.PivotTables.Count);
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
