##Class CharacterBulletValue
Aspose.Cells.Drawing.Texts.CharacterBulletValue class. Represents the character bullet
## CharacterBulletValue class
Represents the character bullet.
```csharp
public class CharacterBulletValue : BulletValue
```
## Constructors
| Name | Description |
| --- | --- |
| [CharacterBulletValue](characterbulletvalue/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Character](../../aspose.cells.drawing.texts/characterbulletvalue/character/) { get; set; } | Gets and sets character of the bullet. |
| override [Type](../../aspose.cells.drawing.texts/characterbulletvalue/type/) { get; } | Gets the type of the bullet. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextsClassCharacterBulletValueDemo
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
workbook.Save("CharacterBulletValueDemo.xlsx");
}
}
}
```
### See Also
* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
