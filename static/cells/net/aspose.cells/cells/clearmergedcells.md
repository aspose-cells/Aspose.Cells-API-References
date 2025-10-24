##Cells.ClearMergedCells
Cells method. Clears all merged ranges
## Cells.ClearMergedCells method
Clears all merged ranges.
```csharp
public void ClearMergedCells()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodClearMergedCellsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create merged cells in A1:B2
worksheet.Cells.Merge(0, 0, 2, 2);
Console.WriteLine($"Merged areas before clearing: {worksheet.Cells.GetMergedAreas().Length}");
try
{
// Clear all merged cells in the worksheet
worksheet.Cells.ClearMergedCells();
Console.WriteLine("Method executed successfully");
Console.WriteLine($"Merged areas after clearing: {worksheet.Cells.GetMergedAreas().Length}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ClearMergedCells method: {ex.Message}");
}
// Save the result
workbook.Save("ClearMergedCellsDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
