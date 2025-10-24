##Bullet.Type
Bullet property. Gets and sets the type of bullet
## Bullet.Type property
Gets and sets the type of bullet.
```csharp
public BulletType Type { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
namespace AsposeCellsExamples
{
public class BulletPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a textbox
int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
TextBox textbox = worksheet.TextBoxes[textboxIndex];
textbox.Text = "Sample text with bullet";
// Configure bullet properties
Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
bullet.Type = BulletType.Character; // Demonstrating Type property usage
((CharacterBulletValue)bullet.BulletValue).Character = '•';
bullet.FontName = "Arial";
// Save the workbook
workbook.Save("BulletPropertyTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [BulletType](../../bullettype/)
* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
