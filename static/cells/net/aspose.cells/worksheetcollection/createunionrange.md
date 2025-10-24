##WorksheetCollection.CreateUnionRange
WorksheetCollection method. Creates a Range object from an address of the range
## WorksheetCollection.CreateUnionRange method
Creates a [`Range`](../../range/) object from an address of the range.
```csharp
public UnionRange CreateUnionRange(string address, int sheetIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| address | String | The address of the range. |
| sheetIndex | Int32 | The sheet index. |
### Return Value
A [`Range`](../../range/) object
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodCreateUnionRangeWithStringInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a union range from address strings
UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
// Set value for the entire union range
unionRange.Value = "Test";
// Apply styling to the union range
Style style = workbook.CreateStyle();
style.Font.Color = System.Drawing.Color.Red;
style.Font.IsBold = true;
unionRange.ApplyStyle(style, new StyleFlag { FontBold = true, FontColor = true });
// Save the workbook
workbook.Save("UnionRangeDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../../unionrange/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
