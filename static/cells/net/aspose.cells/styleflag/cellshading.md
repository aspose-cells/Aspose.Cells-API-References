##StyleFlag.CellShading
StyleFlag property. Cell shading setting will be applied
## StyleFlag.CellShading property
Cell shading setting will be applied.
```csharp
public bool CellShading { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyCellShadingDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
StyleFlag flag = new StyleFlag();
flag.CellShading = true;
Style style = workbook.CreateStyle();
style.Pattern = BackgroundType.Solid;
style.ForegroundColor = Color.Red;
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].PutValue("Test Cell Shading");
cells.ApplyStyle(style, flag);
workbook.Save("CellShadingDemo.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
