##PivotTable.ShowPivotStyleColumnHeader
PivotTable property. Indicates whether the column header in the pivot table should have the style applied
## PivotTable.ShowPivotStyleColumnHeader property
Indicates whether the column header in the pivot table should have the style applied.
```csharp
public bool ShowPivotStyleColumnHeader { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyShowPivotStyleColumnHeaderDemo
{
public static void Run()
{
// Create a new workbook
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
// Add a pivot table
int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Set pivot table style
pivotTable.ShowPivotStyleColumnHeader = true;
pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
// Save the workbook
workbook.Save("PivotTableShowPivotStyleColumnHeaderDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
