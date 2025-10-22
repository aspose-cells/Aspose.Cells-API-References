##ColumnCollection.GetColumnByIndex
ColumnCollection method. Gets the Column object by the position in the list
## ColumnCollection.GetColumnByIndex method
Gets the [`Column`](../../column/) object by the position in the list.
```csharp
public Column GetColumnByIndex(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The position in the list. |
### Return Value
Returns the column object.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ColumnCollectionMethodGetColumnByIndexWithInt32Demo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to column A
worksheet.Cells["A1"].Value = "Aspose.Cells Column Demo";
try
{
// Get column collection reference
ColumnCollection columns = worksheet.Cells.Columns;
// Access column at index 0 (column A) using GetColumnByIndex
Column column = columns.GetColumnByIndex(0);
// Modify column width to demonstrate column access
column.Width = 25;
Console.WriteLine("Modified width of column at index 0 (Column A) to 25 characters.");
}
catch (ArgumentOutOfRangeException ex)
{
Console.WriteLine($"Invalid column index: {ex.Message}");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
// Save the modified workbook
workbook.Save("ColumnCollectionMethodGetColumnByIndexWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
