##StyleFlag.All
StyleFlag property. All properties will be applied
## StyleFlag.All property
All properties will be applied.
```csharp
public bool All { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyAllDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a style with solid red background
Style style = workbook.CreateStyle();
style.Pattern = BackgroundType.Solid;
style.ForegroundColor = Color.Red;
// Create a style flag with All property set to true
StyleFlag styleFlag = new StyleFlag();
styleFlag.All = true;
// Apply the style to the first column
Column column = cells.Columns[0];
column.ApplyStyle(style, styleFlag);
// Verify the style was applied to cells in the column
Cell cell = cells[0, 0];
Style appliedStyle = cell.GetStyle();
Console.WriteLine("Pattern: " + appliedStyle.Pattern);
Console.WriteLine("Color: " + appliedStyle.ForegroundColor);
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
