##Row.ApplyStyle
Row method. Applies formats for a whole row
## Row.ApplyStyle method
Applies formats for a whole row.
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
public class RowMethodApplyStyleWithStyleStyleFlagDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Set HTML content in first cell
sheet.Cells[0, 0].HtmlString = @"<font style=""color: #49c131; font-weight: bold;"">Styled </font><font>text</font>";
// Get the first row and its style
Row row = sheet.Cells.Rows[0];
Style style = row.GetStyle();
// Modify style properties
style.IsTextWrapped = true;
style.HorizontalAlignment = TextAlignmentType.Center;
// Apply style with specific flags (only wrap text will be applied)
row.ApplyStyle(style, new StyleFlag { WrapText = true });
// Auto-fit for demonstration
sheet.AutoFitRows();
sheet.AutoFitColumns();
// Save the workbook
workbook.Save("RowApplyStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
