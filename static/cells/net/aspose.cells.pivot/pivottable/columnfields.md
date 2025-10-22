##PivotTable.ColumnFields
PivotTable property. Returns a PivotFields object that are currently shown as column fields
## PivotTable.ColumnFields property
Returns a PivotFields object that are currently shown as column fields.
```csharp
public PivotFieldCollection ColumnFields { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyColumnFieldsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
var cells = worksheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Sales";
cells["A2"].Value = "Bikes";
cells["B2"].Value = 100;
cells["A3"].Value = "Bikes";
cells["B3"].Value = 200;
cells["A4"].Value = "Cars";
cells["B4"].Value = 300;
cells["A5"].Value = "Cars";
cells["B5"].Value = 400;
cells["A6"].Value = "Trucks";
cells["B6"].Value = 500;
// Add pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row and column fields
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Sales");
// Access and manipulate column field
PivotField columnField = pivotTable.ColumnFields[0];
columnField.FilterByValue(0, PivotFilterType.ValueGreaterThan, 300, 0);
// Calculate and refresh data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableColumnFieldsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
