##Range.ApplyStyle
Range method. Applies formats for a whole range
## Range.ApplyStyle method
Applies formats for a whole range.
```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |
### Remarks
Each cell in this range will contains a [`Style`](../../style/) object. So this is a memory-consuming method. Please use it carefully.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodApplyStyleWithStyleStyleFlagDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Style style = workbook.CreateStyle();
style.HorizontalAlignment = TextAlignmentType.Center;
style.VerticalAlignment = TextAlignmentType.Center;
style.IsTextWrapped = true;
Cells cells = workbook.Worksheets[0].Cells;
cells[0, 0].PutValue("Sample text for style demonstration");
Aspose.Cells.Range range = cells.CreateRange(0, 0, 1, 3);
StyleFlag styleFlag = new StyleFlag();
styleFlag.HorizontalAlignment = true;
styleFlag.VerticalAlignment = true;
styleFlag.WrapText = true;
range.ApplyStyle(style, styleFlag);
workbook.Save("ApplyStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
