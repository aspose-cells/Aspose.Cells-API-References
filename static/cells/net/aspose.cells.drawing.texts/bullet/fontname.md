##Bullet.FontName
Bullet property. Get and sets the name of the font
## Bullet.FontName property
Get and sets the name of the font.
```csharp
public string FontName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class BulletPropertyFontNameDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
TextBox textbox = worksheet.TextBoxes[textboxIndex];
textbox.Text = "Sample text with bullet";
TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
paragraph.LineSpace = 3000;
Bullet bullet = paragraph.Bullet;
bullet.Type = BulletType.Character;
((CharacterBulletValue)bullet.BulletValue).Character = '•';
bullet.FontName = "Arial";
workbook.Save("BulletFontNameDemo.xlsx");
}
}
}
```
### See Also
* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
