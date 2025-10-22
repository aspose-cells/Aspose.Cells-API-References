##Range.Intersect
Range method. Returns a Range object that represents the rectangular intersection of two ranges
## Range.Intersect method
Returns a [`Range`](../) object that represents the rectangular intersection of two ranges.
```csharp
public Range Intersect(Range range)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The intersecting range. |
### Return Value
Returns a [`Range`](../) object
### Remarks
If the two ranges are not intersected, returns null.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodIntersectWithRangeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
Aspose.Cells.Range range1 = cells.CreateRange("A1:A5");
Aspose.Cells.Range range2 = cells.CreateRange("A3:A10");
Aspose.Cells.Range intersectRange = range1.Intersect(range2);
Console.WriteLine("Intersected range: " + intersectRange.Address);
workbook.Save("IntersectDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
