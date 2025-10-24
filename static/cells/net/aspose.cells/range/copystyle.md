##Range.CopyStyle
Range method. Copies style settings from a source range
## Range.CopyStyle method
Copies style settings from a source range.
```csharp
public void CopyStyle(Range range)
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
public class RangeMethodCopyStyleWithRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet sheetSrc = workbook.Worksheets[0];
sheetSrc.Name = "Source";
// Add some sample style to source range
Cells cellsSrc = sheetSrc.Cells;
Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A1:D5");
Style style = workbook.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 14;
style.Font.IsBold = true;
style.ForegroundColor = System.Drawing.Color.Yellow;
style.Pattern = BackgroundType.Solid;
rangeSrc.SetStyle(style);
// Create destination worksheet
Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
sheetDest.Name = "Destination";
// Create destination range and copy style
Cells cellsDest = sheetDest.Cells;
Aspose.Cells.Range rangeDest = cellsDest.CreateRange("A1:D5");
rangeDest.CopyStyle(rangeSrc);
// Save the workbook
workbook.Save("RangeCopyStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
