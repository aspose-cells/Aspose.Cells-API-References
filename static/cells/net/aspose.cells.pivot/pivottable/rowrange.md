##PivotTable.RowRange
PivotTable property. Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Readonly
## PivotTable.RowRange property
Returns a CellArea object that represents the range that contains the row area in the PivotTable report. Read-only.
```csharp
public CellArea RowRange { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyRowRangeDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("example.xlsx");
// Refresh all pivot tables in the workbook
workbook.Worksheets.RefreshAll();
// Get the first pivot table from the first worksheet
PivotTable pivotTable = workbook.Worksheets[0].PivotTables[0];
// Get the row range of the pivot table
CellArea rowRange = pivotTable.RowRange;
// Display the row range coordinates
Console.WriteLine("PivotTable Row Range:");
Console.WriteLine($"Start Row: {rowRange.StartRow}");
Console.WriteLine($"End Row: {rowRange.EndRow}");
Console.WriteLine($"Start Column: {rowRange.StartColumn}");
Console.WriteLine($"End Column: {rowRange.EndColumn}");
// Get the column range of the pivot table
CellArea columnRange = pivotTable.ColumnRange;
// Display the column range coordinates
Console.WriteLine("\nPivotTable Column Range:");
Console.WriteLine($"Start Row: {columnRange.StartRow}");
Console.WriteLine($"End Row: {columnRange.EndRow}");
Console.WriteLine($"Start Column: {columnRange.StartColumn}");
Console.WriteLine($"End Column: {columnRange.EndColumn}");
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
