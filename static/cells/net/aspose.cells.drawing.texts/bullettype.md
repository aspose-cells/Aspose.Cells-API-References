##Enum BulletType
Aspose.Cells.Drawing.Texts.BulletType enum. Represents the type of the bullet
## BulletType enumeration
Represents the type of the bullet.
```csharp
public enum BulletType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No bullet. |
| Character | `1` | Character bullet. |
| Picture | `2` | Image bullet. |
| AutoNumbered | `3` | Automatic numbered bullet. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class TextsClassBulletTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a TextBox and set text
TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
textBox.Text = "Sample text with bullet type demonstration";
// Create bullet options
NoneBulletValue noneBullet = new NoneBulletValue();
BulletType bulletType = noneBullet.Type;
// Apply bullet settings to text paragraphs
foreach (TextParagraph paragraph in textBox.TextBody.TextParagraphs)
{
paragraph.Bullet.Type = bulletType;
}
Console.WriteLine("Bullet Type applied: " + bulletType);
workbook.Save("BulletTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
