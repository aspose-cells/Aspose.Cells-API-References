##PivotTable.ColumnRange
PivotTable property. Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Readonly
## PivotTable.ColumnRange property
Returns a CellArea object that represents the range that contains the column area in the PivotTable report. Read-only.
```csharp
public CellArea ColumnRange { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyColumnRangeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["B1"].Value = "Region";
worksheet.Cells["C1"].Value = "Sales";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["B2"].Value = "North";
worksheet.Cells["C2"].Value = 1000;
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["B3"].Value = "South";
worksheet.Cells["C3"].Value = 2000;
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B4"].Value = "East";
worksheet.Cells["C4"].Value = 3000;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Refresh pivot table data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Get column range of pivot table
CellArea columnRange = pivotTable.ColumnRange;
Console.WriteLine("Pivot Table Column Range: " + columnRange);
// Save the workbook
workbook.Save("PivotTableColumnRangeDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
