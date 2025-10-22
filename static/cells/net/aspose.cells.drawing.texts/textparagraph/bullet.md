##TextParagraph.Bullet
TextParagraph property. Gets the bullet
## TextParagraph.Bullet property
Gets the bullet.
```csharp
public Bullet Bullet { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextParagraphPropertyBulletDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a textbox
int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
TextBox textbox = worksheet.TextBoxes[textboxIndex];
// Set text and configure paragraph
textbox.Text = "First Item\nSecond Item";
textbox.TextBody.TextParagraphs[0].LineSpaceSizeType = LineSpaceSizeType.Percentage;
textbox.TextBody.TextParagraphs[0].LineSpace = 3000;
// Configure bullet for the first paragraph
Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
bullet.Type = BulletType.Character;
((CharacterBulletValue)bullet.BulletValue).Character = '•';
bullet.FontName = "Arial";
// Save the workbook
workbook.Save("TextParagraphPropertyBulletDemo.xlsx");
}
}
}
```
### See Also
* class [Bullet](../../bullet/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
