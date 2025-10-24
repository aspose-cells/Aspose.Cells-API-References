##FontSettingCollection.TextParagraphs
FontSettingCollection property. Gets all paragraphs
## FontSettingCollection.TextParagraphs property
Gets all paragraphs.
```csharp
public TextParagraphCollection TextParagraphs { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class FontSettingCollectionPropertyTextParagraphsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a textbox to the worksheet
int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
TextBox textbox = worksheet.TextBoxes[textboxIndex];
textbox.Text = "First paragraph\nSecond paragraph";
// Access the first text paragraph
TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
// Set line spacing properties
paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
paragraph.LineSpace = 3000; // 300% line spacing
// Set bullet properties
Bullet bullet = paragraph.Bullet;
bullet.Type = BulletType.Character;
((CharacterBulletValue)bullet.BulletValue).Character = '•';
bullet.FontName = "Arial";
// Save the workbook
workbook.Save("TextParagraphsDemo.xlsx");
}
}
}
```
### See Also
* class [TextParagraphCollection](../../textparagraphcollection/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
