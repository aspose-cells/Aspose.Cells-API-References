##StyleFlag.Indent
StyleFlag property. Indent level setting will be applied
## StyleFlag.Indent property
Indent level setting will be applied.
```csharp
public bool Indent { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyIndentDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style with indent level
Style style = workbook.CreateStyle();
style.IndentLevel = 2;
style.HorizontalAlignment = TextAlignmentType.Left;
// Create style flag with Indent property set
StyleFlag styleFlag = new StyleFlag();
styleFlag.Indent = true;
// Apply data to cells
for (int row = 0; row < 5; row++)
{
for (int col = 0; col < 5; col++)
{
worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
}
}
// Apply the style with indent to a range
Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 5, 5);
range.ApplyStyle(style, styleFlag);
// Verify the style was applied
Cell cell = worksheet.Cells["A1"];
Style appliedStyle = cell.GetStyle();
Console.WriteLine($"Indent Level: {appliedStyle.IndentLevel}");
Console.WriteLine($"Alignment: {appliedStyle.HorizontalAlignment}");
// Save the workbook
workbook.Save("IndentStyleDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
