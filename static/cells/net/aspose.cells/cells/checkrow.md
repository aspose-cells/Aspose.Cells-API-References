##Cells.CheckRow
Cells method. Gets the Row element or null at the specified cell row index
## Cells.CheckRow method
Gets the [`Row`](../../row/) element or null at the specified cell row index.
```csharp
public Row CheckRow(int row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index |
### Return Value
Returns [`Row`](../../row/) object If the row object does exist, otherwise returns null.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodCheckRowWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Populate some data
cells["A1"].PutValue("Header");
cells["A2"].PutValue(100);
cells["A3"].PutValue(200);
// Check if row exists and get row object
Row row = cells.CheckRow(1);
if (row != null)
{
Console.WriteLine("Row 1 exists with height: " + row.Height);
}
// Check non-existent row
Row nonExistentRow = cells.CheckRow(100);
Console.WriteLine("Row 100 exists: " + (nonExistentRow != null));
}
}
}
```
### See Also
* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
