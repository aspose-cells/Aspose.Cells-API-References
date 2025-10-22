##Range.Union
Range method. Returns the union of two ranges
## Range.Union method
Returns the union of two ranges.
```csharp
[Obsolete("Use Range.UnionRanges() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList Union(Range range)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range |
### Return Value
The union of two ranges.
### Remarks
NOTE: This method is now obsolete. Instead, please use Range.UnionRanges() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Collections;
public class RangeMethodUnionWithRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two ranges to demonstrate Union
Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B2");
Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:C3");
// Fill some data in the ranges
range1[0, 0].PutValue("Range1");
range2[0, 0].PutValue("Range2");
try
{
// Call the Union method (note: this is the obsolete version)
ArrayList unionResult = range1.Union(range2);
Console.WriteLine("Union method executed successfully");
Console.WriteLine($"Number of ranges in union: {unionResult.Count}");
// Display addresses of all ranges in the union
foreach (Aspose.Cells.Range r in unionResult)
{
Console.WriteLine($"Union range address: {r.Address}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Union method: {ex.Message}");
}
// Save the result
workbook.Save("RangeMethodUnionWithRangeDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
