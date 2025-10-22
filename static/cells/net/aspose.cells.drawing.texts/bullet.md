##Class Bullet
Aspose.Cells.Drawing.Texts.Bullet class. Represents the bullet points should be applied to a paragraph
## Bullet class
Represents the bullet points should be applied to a paragraph.
```csharp
public class Bullet
```
## Properties
| Name | Description |
| --- | --- |
| [BulletValue](../../aspose.cells.drawing.texts/bullet/bulletvalue/) { get; } | Gets the value of bullet. |
| [FontName](../../aspose.cells.drawing.texts/bullet/fontname/) { get; set; } | Get and sets the name of the font. |
| [Type](../../aspose.cells.drawing.texts/bullet/type/) { get; set; } | Gets and sets the type of bullet. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextsClassBulletDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
TextBox textbox = worksheet.TextBoxes[textboxIndex];
textbox.Text = "Sample text";
TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
paragraph.LineSpace = 3000;
Bullet bullet = paragraph.Bullet;
bullet.Type = BulletType.Character;
((CharacterBulletValue)bullet.BulletValue).Character = 'v';
bullet.FontName = "Arial";
workbook.Save("TextsClassBulletDemo_Output.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
