##StyleFlag.TopBorder
StyleFlag property. Top border settings will be applied
## StyleFlag.TopBorder property
Top border settings will be applied.
```csharp
public bool TopBorder { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyTopBorderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create a style with top border settings
Style style = workbook.CreateStyle();
style.Borders[BorderType.TopBorder].Color = Color.Red;
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Dashed;
// Create style flag and enable top border modification
StyleFlag styleFlag = new StyleFlag();
styleFlag.TopBorder = true;
// Apply the style to cell A1 with only top border flag enabled
Cell cell = sheet.Cells["A1"];
cell.PutValue("Sample Text");
cell.SetStyle(style, styleFlag);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
