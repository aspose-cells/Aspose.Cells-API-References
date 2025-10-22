##StyleFlag.WrapText
StyleFlag property. Wrap text setting will be applied
## StyleFlag.WrapText property
Wrap text setting will be applied.
```csharp
public bool WrapText { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyWrapTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style with text wrapping enabled
Style style = workbook.CreateStyle();
style.IsTextWrapped = true;
// Create a style flag and enable WrapText flag
StyleFlag flag = new StyleFlag();
flag.WrapText = true;
// Apply the style to cell A1 with the specified flags
worksheet.Cells["A1"].PutValue("This is a long text that should wrap in the cell");
worksheet.Cells.ApplyStyle(style, flag);
// Auto-fit row height to see the wrapped text
worksheet.AutoFitRow(0);
// Save the workbook
workbook.Save("WrapTextDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
