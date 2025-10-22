##StyleFlag.FontColor
StyleFlag property. Font color setting will be applied
## StyleFlag.FontColor property
Font color setting will be applied.
```csharp
public bool FontColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyFontColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a custom style
Style style = workbook.CreateStyle();
style.Font.Color = System.Drawing.Color.Red;
style.BackgroundColor = System.Drawing.Color.LightGray;
// Create style flag and enable font color and cell shading
StyleFlag styleFlag = new StyleFlag();
styleFlag.FontColor = true;
styleFlag.CellShading = true;
// Apply the style to cell A1 with the specified flags
worksheet.Cells["A1"].PutValue("Red Text on Gray Background");
worksheet.Cells["A1"].SetStyle(style, styleFlag);
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
