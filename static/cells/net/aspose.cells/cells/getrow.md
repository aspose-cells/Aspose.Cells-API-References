##Cells.GetRow
Cells method. Gets the Row element at the specified cell row index
## Cells.GetRow method
Gets the [`Row`](../../row/) element at the specified cell row index.
```csharp
[Obsolete("Use Cells.CheckRow(int row) instead.")]
public Row GetRow(int row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |
### Return Value
If the row object does exist return Row object, otherwise return null.
### Remarks
NOTE: This member is now obsolete. Instead, please use Cells.CheckRow(int row) method. This method will be removed 12 months later since February 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodGetRowWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create cells in row 5 to ensure the row exists
worksheet.Cells["A5"].PutValue("Row 5 Data");
worksheet.Cells["B5"].PutValue(12345);
try
{
// Call GetRow method with Int32 parameter
Row resultRow = worksheet.Cells.GetRow(5);
if (resultRow != null)
{
// Demonstrate row manipulation
resultRow.Height = 20;
Console.WriteLine($"Retrieved row 5 successfully. Current height: {resultRow.Height} points");
// Count cells in the row
int cellCount = 0;
foreach (Cell cell in resultRow)
{
cellCount++;
}
Console.WriteLine($"Row 5 contains {cellCount} cells");
}
else
{
Console.WriteLine("Row 5 not found in worksheet");
}
}
catch (ArgumentOutOfRangeException ex)
{
Console.WriteLine($"Invalid row index: {ex.Message}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetRow: {ex.Message}");
}
// Save the modified workbook
workbook.Save("CellsMethodGetRowWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
