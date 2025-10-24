##UnionRange.HasRange
UnionRange property. Indicates whether this has range
## UnionRange.HasRange property
Indicates whether this has range.
```csharp
public bool HasRange { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class UnionRangePropertyHasRangeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a union range using the correct API
UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
// Check if the union range has valid ranges
Console.WriteLine("UnionRange has ranges: " + unionRange.HasRange);
// Set value and style only if the range is valid
if (unionRange.HasRange)
{
unionRange.Value = "Test Value";
Style style = workbook.CreateStyle();
style.Pattern = BackgroundType.Solid;
style.ForegroundColor = System.Drawing.Color.LightBlue;
unionRange.ApplyStyle(style, new StyleFlag { All = true });
}
workbook.Save("UnionRangeHasRangeDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
