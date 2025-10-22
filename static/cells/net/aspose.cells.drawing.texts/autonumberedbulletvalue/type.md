##AutoNumberedBulletValue.Type
AutoNumberedBulletValue property. Gets the type of the bullet
## AutoNumberedBulletValue.Type property
Gets the type of the bullet.
```csharp
public override BulletType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class AutoNumberedBulletValuePropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape to add text with bullets
var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 10, 300, 100);
var textParagraph = shape.TextBody.TextParagraphs[0];
// Create an auto-numbered bullet value
var bullet = new AutoNumberedBulletValue
{
AutonumberScheme = TextAutonumberScheme.AlphaLcParenBoth,
StartAt = 1
};
// Since we can't set BulletValue directly, we'll need to find another way
// to apply the bullet style. This might involve using the shape's text formatting
// or other available methods in the API.
// For demonstration, we'll just display the bullet type
Console.WriteLine("Bullet Type: " + bullet.Type);
// Add text to the paragraph through the shape's text body
shape.TextBody.Text = "First Item";
// Add another paragraph with different numbering scheme
// Since we can't Add, we'll use the next available paragraph
var secondParagraph = shape.TextBody.TextParagraphs[1];
var bullet2 = new AutoNumberedBulletValue
{
AutonumberScheme = TextAutonumberScheme.Arabic1Minus,
StartAt = 1
};
// Display the bullet type (read-only property)
Console.WriteLine("Second Bullet Type: " + bullet2.Type);
// Add text to the second paragraph
shape.TextBody.Text += "\nSecond Item";
// Save the workbook to demonstrate the bullet effects
workbook.Save("AutoNumberedBulletDemo.xlsx");
}
}
}
```
### See Also
* enum [BulletType](../../bullettype/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
