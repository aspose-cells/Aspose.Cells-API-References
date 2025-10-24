##StyleFlag.Font
StyleFlag property. Font settings will be applied
## StyleFlag.Font property
Font settings will be applied.
```csharp
public bool Font { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyFontDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
var shape = workbook.Worksheets[0].Shapes.AddButton(0, 0, 100, 100, 100, 100);
shape.Text = "Sample Text";
Aspose.Cells.Font font = workbook.CreateStyle().Font;
font.Name = "Arial";
font.Size = 14;
font.Color = Color.Blue;
font.IsBold = true;
StyleFlag flag = new StyleFlag();
flag.Font = true;
shape.FormatCharacters(0, shape.Text.Length, font, flag);
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
