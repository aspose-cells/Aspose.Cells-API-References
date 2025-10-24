##PivotField.AutoShowCount
PivotField property. Represent the number of top or bottom items that are automatically shown in the specified PivotTable field
## PivotField.AutoShowCount property
Represent the number of top or bottom items that are automatically shown in the specified PivotTable field.
```csharp
public int AutoShowCount { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyAutoShowCountDemo
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
cells["B6"].Value = 25;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field and set AutoShow properties
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
PivotField rowField = pivotTable.RowFields[0];
rowField.AutoShowCount = 2;
rowField.IsAutoShow = true;
rowField.AutoShowField = 1; // Index of "Quantity" field (0-based)
// Calculate data and save
pivotTable.CalculateData();
workbook.Save("PivotFieldAutoShowCountDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
