##PivotTable.ClearData
PivotTable method. Clear PivotTables data and formatting
## PivotTable.ClearData method
Clear PivotTable's data and formatting
```csharp
public void ClearData()
```
### Remarks
If this method is not called before you add or delete PivotField, Maybe the PivotTable data is not corrected
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodClearDataDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Fruit");
worksheet.Cells["A3"].PutValue("Fruit");
worksheet.Cells["A4"].PutValue("Vegetable");
worksheet.Cells["B1"].PutValue("Amount");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(15);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
pivotTable.RefreshData();
pivotTable.CalculateData();
Console.WriteLine("Pivot table with data:");
Console.WriteLine(worksheet.Cells["D1"].StringValue);
Console.WriteLine(worksheet.Cells["D2"].StringValue);
Console.WriteLine(worksheet.Cells["D3"].StringValue);
// Clear pivot table data
pivotTable.ClearData();
Console.WriteLine("\nAfter ClearData():");
Console.WriteLine("Pivot table row count: " + (pivotTable.DataBodyRange.EndRow - pivotTable.DataBodyRange.StartRow + 1));
// Rebuild pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
pivotTable.RefreshData();
pivotTable.CalculateData();
Console.WriteLine("\nRebuilt pivot table:");
Console.WriteLine(worksheet.Cells["D1"].StringValue);
Console.WriteLine(worksheet.Cells["D2"].StringValue);
Console.WriteLine(worksheet.Cells["D3"].StringValue);
// Save workbook
workbook.Save("PivotTableClearDataDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
