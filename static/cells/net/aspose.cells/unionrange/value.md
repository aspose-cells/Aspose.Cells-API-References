##UnionRange.Value
UnionRange property. Gets and sets the values of the range
## UnionRange.Value property
Gets and sets the values of the range.
```csharp
public object Value { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class UnionRangePropertyValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a union range using the correct API
UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:B2,D1:E2", 0);
// Set value for the entire union range
unionRange.Value = "Test Value";
// Create and apply style
Style style = workbook.CreateStyle();
style.Pattern = BackgroundType.Solid;
style.ForegroundColor = System.Drawing.Color.LightBlue;
unionRange.ApplyStyle(style, new StyleFlag { All = true });
// Save the workbook
workbook.Save("UnionRangeValueDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
