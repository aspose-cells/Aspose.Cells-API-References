##PivotTable.EnableFieldDialog
PivotTable property. Indicates whether the PivotTable Field dialog box is available when the user doubleclicks the PivotTable field
## PivotTable.EnableFieldDialog property
Indicates whether the PivotTable Field dialog box is available when the user double-clicks the PivotTable field.
```csharp
public bool EnableFieldDialog { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyEnableFieldDialogDemo
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
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 15;
cells["A4"].Value = "Banana";
cells["B4"].Value = 20;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Demonstrate EnableFieldDialog property
pivotTable.EnableFieldDialog = true;
Console.WriteLine("EnableFieldDialog set to: " + pivotTable.EnableFieldDialog);
// Change the property and verify
pivotTable.EnableFieldDialog = false;
Console.WriteLine("EnableFieldDialog changed to: " + pivotTable.EnableFieldDialog);
// Save the workbook
workbook.Save("PivotTable_EnableFieldDialog_Example.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
