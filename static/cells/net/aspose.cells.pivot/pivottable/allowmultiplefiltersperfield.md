##PivotTable.AllowMultipleFiltersPerField
PivotTable property. Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them
## PivotTable.AllowMultipleFiltersPerField property
Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.
```csharp
public bool AllowMultipleFiltersPerField { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyAllowMultipleFiltersPerFieldDemo
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
cells["B3"].Value = 20;
cells["A4"].Value = "Banana";
cells["B4"].Value = 15;
cells["A5"].Value = "Apple";
cells["B5"].Value = 5;
cells["A6"].Value = "Orange";
cells["B6"].Value = 10;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Set AllowMultipleFiltersPerField property
pivotTable.AllowMultipleFiltersPerField = true;
Console.WriteLine("AllowMultipleFiltersPerField: " + pivotTable.AllowMultipleFiltersPerField);
// Save the workbook
workbook.Save("PivotTable_AllowMultipleFiltersPerField.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
