##PivotTable.ShowRowGrandTotals
PivotTable property. Indicates whether to show grand totals for rows of the pivot table
## PivotTable.ShowRowGrandTotals property
Indicates whether to show grand totals for rows of the pivot table.
```csharp
public bool ShowRowGrandTotals { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyShowRowGrandTotalsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Region";
cells["C1"].Value = "Sales";
cells["A2"].Value = "Product A";
cells["B2"].Value = "North";
cells["C2"].Value = 1000;
cells["A3"].Value = "Product B";
cells["B3"].Value = "South";
cells["C3"].Value = 1500;
cells["A4"].Value = "Product A";
cells["B4"].Value = "South";
cells["C4"].Value = 2000;
cells["A5"].Value = "Product B";
cells["B5"].Value = "North";
cells["C5"].Value = 1200;
// Add a pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Configure pivot table
pivotTable.ShowRowGrandTotals = true; // Demonstrate ShowRowGrandTotals property
pivotTable.ShowColumnGrandTotals = true;
// Add fields to areas
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
// Save the workbook
workbook.Save("PivotTableShowRowGrandTotalsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
