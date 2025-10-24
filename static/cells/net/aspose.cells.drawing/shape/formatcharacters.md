##Shape.FormatCharacters
Shape method. Formats some characters with the font setting
## Shape.FormatCharacters method
Formats some characters with the font setting.
```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | The start index. |
| length | Int32 | The length. |
| font | Font | The font setting. |
| flag | StyleFlag | The flag of the font setting. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
textBox.Text = "Sample Text Formatting";
// Create a font with desired properties
Aspose.Cells.Font font = textBox.Font;
font.Name = "Arial";
font.Size = 12;
font.IsBold = true;
// Create style flag to specify which properties to apply
StyleFlag flag = new StyleFlag();
flag.FontName = true;
flag.FontSize = true;
flag.FontBold = true;
// Apply formatting to specific characters
textBox.FormatCharacters(0, 6, font, flag);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
