##PivotTable.DataBodyRange
PivotTable property. Returns a CellArea object that represents the range that contains the data area in the list between the header row and the insert row. Readonly
## PivotTable.DataBodyRange property
Returns a [`CellArea`](../../../aspose.cells/cellarea/) object that represents the range that contains the data area in the list between the header row and the insert row. Read-only.
```csharp
public CellArea DataBodyRange { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyDataBodyRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Cells cells = sheet.Cells;
// Add sample data for pivot table
cells["A1"].Value = "Product";
cells["B1"].Value = "Sales";
cells["A2"].Value = "Bike";
cells["B2"].Value = 1000;
cells["A3"].Value = "Car";
cells["B3"].Value = 2000;
cells["A4"].Value = "Bike";
cells["B4"].Value = 1500;
cells["A5"].Value = "Car";
cells["B5"].Value = 2500;
// Add pivot table
int pivotIndex = sheet.PivotTables.Add("A7", "A1:B5", "PivotTable1");
PivotTable pivot = sheet.PivotTables[pivotIndex];
// Configure pivot table
pivot.AddFieldToArea(PivotFieldType.Row, "Product");
pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
// Refresh pivot table data
pivot.RefreshData();
pivot.CalculateData();
// Demonstrate DataBodyRange usage
CellArea dataBodyArea = pivot.DataBodyRange;
Console.WriteLine($"Data body range: StartRow={dataBodyArea.StartRow}, EndRow={dataBodyArea.EndRow}, StartColumn={dataBodyArea.StartColumn}, EndColumn={dataBodyArea.EndColumn}");
// Save the workbook
workbook.Save("PivotTableDataBodyRangeDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
