##ColumnCollection.GetByIndex
ColumnCollection method. Gets the column object by the index
## ColumnCollection.GetByIndex method
Gets the column object by the index.
```csharp
[Obsolete("Use Columns.GetColumnByIndex() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Column GetByIndex(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 |  |
### Return Value
Returns the column object.
### Remarks
NOTE: This member is now obsolete. Instead, please use Columns.GetColumnByIndex() method. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ColumnCollectionMethodGetByIndexWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create columns in the collection by setting widths
worksheet.Cells.Columns[0].Width = 15;  // Column 0
worksheet.Cells.Columns[2].Width = 20;  // Column 2
worksheet.Cells.Columns[4].Width = 25;  // Column 4
try
{
// Get second column from ColumnCollection (index 1)
Column column = worksheet.Cells.Columns.GetByIndex(1);
Console.WriteLine($"Retrieved column at collection index 1");
Console.WriteLine($"Worksheet column index: {column.Index}");
Console.WriteLine($"Original width: {column.Width}");
// Modify the retrieved column
column.Width = 35;
Console.WriteLine($"Updated width: {column.Width}");
}
catch (ArgumentOutOfRangeException ex)
{
Console.WriteLine($"Invalid index: {ex.Message}");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
workbook.Save("ColumnCollectionGetByIndexDemo.xlsx");
}
}
}
```
### See Also
* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
