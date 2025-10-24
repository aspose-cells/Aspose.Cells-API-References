##Column.ApplyStyle
Column method. Applies formats for a whole column
## Column.ApplyStyle method
Applies formats for a whole column.
```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ColumnMethodApplyStyleWithStyleStyleFlagDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Set multi-line text in column 2
sheet.Cells[0, 1].Value = "Line1\nLine2";
sheet.Cells[1, 1].Value = "Text with\nmultiple lines";
sheet.Cells[2, 1].Value = "Another\nmulti-line\ntext";
// Create style with wrap text enabled
Style style = workbook.CreateStyle();
style.IsTextWrapped = true;
// Apply style only to wrap text property of column 2
sheet.Cells.Columns[1].ApplyStyle(style, new StyleFlag() { WrapText = true });
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
