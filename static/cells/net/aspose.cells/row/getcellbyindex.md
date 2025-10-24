##Row.GetCellByIndex
Row method. Get the cell by specific index in the cells collection of this row
## Row.GetCellByIndex method
Get the cell by specific index in the cells collection of this row.
```csharp
public Cell GetCellByIndex(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index(position) of the cell in the cells collection of this row. |
### Return Value
The Cell object at given position.
### Remarks
To traverse all cells in sequence without modification, using [`GetEnumerator`](../getenumerator/) will give better performance than using this method to get cell one by one.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowMethodGetCellByIndexWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add data to cells in first row
worksheet.Cells["A1"].PutValue("Cell A1");
worksheet.Cells["B1"].PutValue("Cell B1");
worksheet.Cells["C1"].PutValue("Cell C1");
// Get first row
Row row = worksheet.Cells.Rows[0];
// Demonstrate GetCellByIndex with Int32 parameter
Cell cellAtIndex0 = row.GetCellByIndex(0);
Cell cellAtIndex1 = row.GetCellByIndex(1);
Cell cellAtIndex2 = row.GetCellByIndex(2);
Console.WriteLine("Cell at index 0: " + cellAtIndex0.StringValue);
Console.WriteLine("Cell at index 1: " + cellAtIndex1.StringValue);
Console.WriteLine("Cell at index 2: " + cellAtIndex2.StringValue);
workbook.Save("RowGetCellByIndexDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
