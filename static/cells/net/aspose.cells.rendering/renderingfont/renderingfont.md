##RenderingFont.RenderingFont
RenderingFont constructor. Initializes a new instance of the RenderingFont
## RenderingFont constructor
Initializes a new instance of the [`RenderingFont`](../)
```csharp
public RenderingFont(string fontName, float fontSize)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fontName | String | font name |
| fontSize | Single | font size in points |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;
namespace AsposeCellsExamples
{
public class RenderingFontMethodCtorWithStringSingleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a font using #ctor(string, single) constructor
RenderingFont font = new RenderingFont("Arial", 24f);
font.Bold = true;
font.Color = System.Drawing.Color.Red;
// Create style and set font
Style style = workbook.CreateStyle();
style.Font.Name = font.Name;
style.Font.Size = (int)font.Size;  // Explicit cast from float to int
style.Font.IsBold = font.Bold;
style.Font.Color = font.Color;
// Apply style to cell
worksheet.Cells["A1"].PutValue("Text with custom font");
worksheet.Cells["A1"].SetStyle(style);
// Save the workbook
workbook.Save("FontDemoOutput.xlsx");
}
}
}
```
### See Also
* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
