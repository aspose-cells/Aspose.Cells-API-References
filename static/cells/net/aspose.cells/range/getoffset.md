##Range.GetOffset
Range method. Gets Range range by offset
## Range.GetOffset method
Gets [`Range`](../) range by offset.
```csharp
public Range GetOffset(int rowOffset, int columnOffset)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | Row offset in this range, zero based. |
| columnOffset | Int32 | Column offset in this range, zero based. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodGetOffsetWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create initial range
Aspose.Cells.Range originalRange = cells.CreateRange("A1");
Console.WriteLine("Original Range Address: " + originalRange.Address);
// Get offset range
Aspose.Cells.Range offsetRange = originalRange.GetOffset(1, 1);
Console.WriteLine("Offset Range Address: " + offsetRange.Address);
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
