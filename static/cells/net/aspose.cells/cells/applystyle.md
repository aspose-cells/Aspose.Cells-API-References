##Cells.ApplyStyle
Cells method. Applies formats for a whole worksheet
## Cells.ApplyStyle method
Applies formats for a whole worksheet.
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
public class CellsMethodApplyStyleWithStyleStyleFlagDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Access first worksheet
Worksheet sheet = wb.Worksheets[0];
// Create a style and set text wrapping
Style style = wb.CreateStyle();
style.IsTextWrapped = true;
// Create style flag and enable text wrap flag
StyleFlag flag = new StyleFlag();
flag.WrapText = true;
// Apply the style to all cells in the worksheet
sheet.Cells.ApplyStyle(style, flag);
// Save the workbook
wb.Save("output.xlsx", SaveFormat.Xlsx);
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
