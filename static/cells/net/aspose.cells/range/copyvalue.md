##Range.CopyValue
Range method. Copies cell value from a source range
## Range.CopyValue method
Copies cell value from a source range.
```csharp
public void CopyValue(Range range)
```
| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source [`Range`](../) object. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodCopyValueWithRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and get the first worksheet
Worksheet sheetSrc = workbook.Worksheets[0];
sheetSrc.Name = "SourceSheet";
// Add another worksheet for destination
Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
sheetDest.Name = "DestinationSheet";
// Create sample data in source range
Cells cellsSrc = sheetSrc.Cells;
cellsSrc["A1"].PutValue("Source Data");
cellsSrc["A2"].PutValue(10);
cellsSrc["B2"].PutValue(20);
cellsSrc["A3"].PutValue(30);
cellsSrc["B3"].PutValue(40);
// Create ranges for source and destination
Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A2:B3");
Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("D2:E3");
// Copy values from source range to destination range
rangeDest.CopyValue(rangeSrc);
// Save the workbook
workbook.Save("RangeCopyValueDemo.xlsx");
Console.WriteLine("Values copied successfully from source range to destination range.");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
