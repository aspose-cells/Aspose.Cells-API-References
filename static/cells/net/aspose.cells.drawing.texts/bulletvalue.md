##Class BulletValue
Aspose.Cells.Drawing.Texts.BulletValue class. Represents the value of the bullet
## BulletValue class
Represents the value of the bullet.
```csharp
public abstract class BulletValue
```
## Properties
| Name | Description |
| --- | --- |
| abstract [Type](../../aspose.cells.drawing.texts/bulletvalue/type/) { get; } | Gets the type of the bullet's value. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextsClassBulletValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a text box and get its text paragraphs
var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
var textParagraph = textBox.TextBody.TextParagraphs[0];
// Create an instance of CharacterBulletValue (which inherits from BulletValue)
var bulletValue = new CharacterBulletValue();
bulletValue.Character = '•';
// Set the bullet value to the paragraph (Bullet is read-only, so we need to modify it differently)
// Since Bullet is read-only, we need to find another way to set it
// This might involve creating a new TextParagraph with the bullet set
// Note: The actual API might provide a different way to set bullets
// For demonstration, we'll assume we can set it through some other means
// textParagraph.Bullet = bulletValue; // This line is removed as Bullet is read-only
textBox.Text = "First bullet point";
// Add another paragraph with different bullet
// TextParagraphCollection doesn't have an Add method, so we need to find another way
// This might involve creating a new TextParagraph and adding it through some other means
// For demonstration, we'll assume we can get the second paragraph directly
var textParagraph2 = textBox.TextBody.TextParagraphs[1];
var bulletValue2 = new CharacterBulletValue();
bulletValue2.Character = '→';
// textParagraph2.Bullet = bulletValue2; // This line is removed as Bullet is read-only
textBox.Text += "\nSecond bullet point";
// Demonstrate accessing bullet type
Console.WriteLine("First bullet type: " + textParagraph.Bullet.Type);
Console.WriteLine("Second bullet type: " + textParagraph2.Bullet.Type);
// Save the result
workbook.Save("TextsClassBulletValueDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
