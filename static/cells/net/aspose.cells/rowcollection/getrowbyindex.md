##RowCollection.GetRowByIndex
RowCollection method. Gets the row object by the position in the list
## RowCollection.GetRowByIndex method
Gets the row object by the position in the list.
```csharp
public Row GetRowByIndex(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The position. |
### Return Value
The Row object at given position.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowCollectionMethodGetRowByIndexWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Get row by index (0-based)
Row row = sheet.Cells.Rows.GetRowByIndex(0);
if (row == null)
{
Console.WriteLine("Row at index 0 is null (not created yet)");
}
else
{
Console.WriteLine("Row at index 0 exists");
}
}
}
}
```
### See Also
* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
