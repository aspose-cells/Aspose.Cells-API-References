##PivotTable.ShowColumnGrandTotals
PivotTable property. Indicates whether to show grand totals for columns of this pivot table
## PivotTable.ShowColumnGrandTotals property
Indicates whether to show grand totals for columns of this pivot table.
```csharp
public bool ShowColumnGrandTotals { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyShowColumnGrandTotalsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
var cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["A3"].Value = "Orange";
cells["A4"].Value = "Banana";
cells["A5"].Value = "Apple";
cells["B2"].Value = 5;
cells["B3"].Value = 3;
cells["B4"].Value = 6;
cells["B5"].Value = 2;
// Add pivot table
int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit as rows
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sum of Quantity
// Demonstrate ShowColumnGrandTotals property
pivotTable.ShowColumnGrandTotals = false; // Disable column grand totals
Console.WriteLine("Column Grand Totals Visible: " + pivotTable.ShowColumnGrandTotals);
// Save the workbook
workbook.Save("PivotTableShowColumnGrandTotalsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
