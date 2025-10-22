##Cells.ApplyRowStyle
Cells method. Applies formats for a whole row
## Cells.ApplyRowStyle method
Applies formats for a whole row.
```csharp
public void ApplyRowStyle(int row, Style style, StyleFlag flag)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodApplyRowStyleWithInt32StyleStyleFlagDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a style with borders
Style style = workbook.CreateStyle();
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
// Create style flag for borders
StyleFlag styleFlag = new StyleFlag();
styleFlag.Borders = true;
// Apply the style to the first row
cells.ApplyRowStyle(0, style, styleFlag);
// Save the workbook
workbook.Save("ApplyRowStyleDemo.xlsx");
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
