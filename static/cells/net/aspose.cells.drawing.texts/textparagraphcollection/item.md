##TextParagraphCollection.Item
TextParagraphCollection property. Gets the TextParagraph object at specific index
## TextParagraphCollection indexer
Gets the [`TextParagraph`](../../textparagraph/) object at specific index.
```csharp
public TextParagraph this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextParagraphCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
TextBox textbox0 = worksheet.TextBoxes[textboxIndex];
textbox0.Text = "Sample text";
// Access paragraph using Item property
TextParagraph paragraph = textbox0.TextBody.TextParagraphs[0];
paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
paragraph.LineSpace = 3000;
Bullet bullet = paragraph.Bullet;
bullet.Type = BulletType.Character;
((CharacterBulletValue)bullet.BulletValue).Character = 'v';
bullet.FontName = "Arial";
workbook.Save("TextParagraphCollectionPropertyItemDemo.xlsx");
}
}
}
```
### See Also
* class [TextParagraph](../../textparagraph/)
* class [TextParagraphCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
