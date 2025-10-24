##PivotTable.TableRange2
PivotTable property. Returns a CellArea object that represents the range containing the entire PivotTable report includes page fields. Readonly
## PivotTable.TableRange2 property
Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read-only.
```csharp
public CellArea TableRange2 { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyTableRange2Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 1000;
worksheet.Cells["B3"].Value = 2000;
worksheet.Cells["B4"].Value = 3000;
// Add a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Get the TableRange2 which includes the entire pivot table
CellArea tableRange2 = pivotTable.TableRange2;
Console.WriteLine($"TableRange2: StartRow={tableRange2.StartRow}, StartColumn={tableRange2.StartColumn}, " +
$"EndRow={tableRange2.EndRow}, EndColumn={tableRange2.EndColumn}");
// Create a range based on TableRange2
Aspose.Cells.Range pivotRange = worksheet.Cells.CreateRange(
tableRange2.StartRow,
tableRange2.StartColumn,
tableRange2.EndRow - tableRange2.StartRow + 1,
tableRange2.EndColumn - tableRange2.StartColumn + 1);
// Output the range address
Console.WriteLine($"Pivot Table Range: {pivotRange.Address}");
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
