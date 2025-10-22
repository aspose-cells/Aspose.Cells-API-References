##Cells.CheckColumn
Cells method. Gets the Column element or null at the specified column index
## Cells.CheckColumn method
Gets the [`Column`](../../column/) element or null at the specified column index.
```csharp
public Column CheckColumn(int columnIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | The column index. |
### Return Value
The Column object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodCheckColumnWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Set a value in column 1 (B3)
cells["B3"].PutValue("Sample Data");
// Check column 4 (E column)
Column column = cells.CheckColumn(4);
// Output column properties
Console.WriteLine("Column Width: " + column.Width);
Console.WriteLine("Column Index: " + column.Index);
}
}
}
```
### See Also
* class [Column](../../column/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
