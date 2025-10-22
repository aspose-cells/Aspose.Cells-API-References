##PivotTable.HasBlankRows
PivotTable property. Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows
## PivotTable.HasBlankRows property
Indicates whether to add blank rows. This property only applies for the PivotTable auto format types which needs to add blank rows.
```csharp
public bool HasBlankRows { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyHasBlankRowsDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet dataSheet = wb.Worksheets[0];
// Create sample data
dataSheet.Cells[0, 0].PutValue("Category");
dataSheet.Cells[0, 1].PutValue("Product");
dataSheet.Cells[0, 2].PutValue("Sales");
Random rnd = new Random();
for (int i = 1; i <= 10; i++)
{
dataSheet.Cells[i, 0].PutValue(rnd.Next(2) == 0 ? "Electronics" : "Furniture");
dataSheet.Cells[i, 1].PutValue("Product " + rnd.Next(1, 4));
dataSheet.Cells[i, 2].PutValue(rnd.Next(100, 1000));
}
// Add pivot table
Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
int pivotIndex = pivotSheet.PivotTables.Add(
"=Sheet1!A1:C11", "A1", "PivotTable1");
PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales
// Demonstrate HasBlankRows property
pivotTable.HasBlankRows = false; // Remove blank lines between items
// Save the workbook
wb.Save("PivotTableHasBlankRowsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
