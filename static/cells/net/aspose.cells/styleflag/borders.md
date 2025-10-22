##StyleFlag.Borders
StyleFlag property. All borders settings will be applied
## StyleFlag.Borders property
All borders settings will be applied.
```csharp
public bool Borders { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyBordersDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a style with border settings
Style style = workbook.CreateStyle();
style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.BottomBorder].Color = System.Drawing.Color.Blue;
// Create a style flag and enable borders
StyleFlag styleFlag = new StyleFlag();
styleFlag.Borders = true;
// Apply the style to cell A1 with borders only
cells["A1"].PutValue("Borders Demo");
cells["A1"].SetStyle(style, styleFlag);
// Save the workbook
workbook.Save("BordersDemo.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
