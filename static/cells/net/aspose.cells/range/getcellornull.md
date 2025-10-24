##Range.GetCellOrNull
Range method. Gets Cell object or null in this range
## Range.GetCellOrNull method
Gets [`Cell`](../../cell/) object or null in this range.
```csharp
public Cell GetCellOrNull(int rowOffset, int columnOffset)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | Row offset in this range, zero based. |
| columnOffset | Int32 | Column offset in this range, zero based. |
### Return Value
[`Cell`](../../cell/) object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodGetCellOrNullWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
// Fill some data in the range
range[0, 0].PutValue("Cell A1");
range[0, 1].PutValue("Cell B1");
range[1, 0].PutValue("Cell A2");
// Demonstrate GetCellOrNull with Int32 parameters
Cell cell1 = range.GetCellOrNull(0, 0);
Console.WriteLine("Cell (0,0): " + (cell1 != null ? cell1.StringValue : "null"));
Cell cell2 = range.GetCellOrNull(1, 1);
Console.WriteLine("Cell (1,1): " + (cell2 != null ? cell2.StringValue : "null"));
// Try to get a cell outside the range (should return null)
Cell cell3 = range.GetCellOrNull(2, 0);
Console.WriteLine("Cell (2,0): " + (cell3 != null ? cell3.StringValue : "null"));
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
