##Cells.ApplyColumnStyle
Cells method. Applies formats for a whole column
## Cells.ApplyColumnStyle method
Applies formats for a whole column.
```csharp
public void ApplyColumnStyle(int column, Style style, StyleFlag flag)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The column index. |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodApplyColumnStyleWithInt32StyleStyleFlagDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Create a style with borders
Style style = workbook.CreateStyle();
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
// Create a style flag to apply only borders
StyleFlag sflag = new StyleFlag();
sflag.Borders = true;
// Apply the style to column 1 (index 0)
cells.ApplyColumnStyle(0, style, sflag);
// Save the workbook
workbook.Save("ApplyColumnStyleOutput.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
