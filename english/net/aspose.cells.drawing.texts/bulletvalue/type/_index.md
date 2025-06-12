---
title: BulletValue.Type
second_title: Aspose.Cells for .NET API Reference
description: BulletValue property. Gets the type of the bullets value
type: docs
url: /net/aspose.cells.drawing.texts/bulletvalue/type/
---
## BulletValue.Type property

Gets the type of the bullet's value.

```csharp
public abstract BulletType Type { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class BulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a text box with bullet points
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 200, 100, 200);
            var textParagraph = textBox.TextBody.TextParagraphs[0];
            
            // Create a bullet with character type
            var bullet = textParagraph.Bullet;
            bullet.Type = BulletType.Character;
            bullet.FontName = "•"; // Changed from Character to FontName
            
            // Display the bullet type
            Console.WriteLine("Bullet Type: " + bullet.Type);

            // Add text to demonstrate the bullet
            textBox.Text = "Item 1";

            // Create another paragraph with different bullet type
            var secondParagraph = textBox.TextBody.TextParagraphs[0]; // Changed from Add to accessing index
            var secondBullet = secondParagraph.Bullet;
            secondBullet.Type = BulletType.AutoNumbered;
            // AutoNumberedBulletStyle is not available in the provided types
            
            // Display the second bullet type
            Console.WriteLine("Second Bullet Type: " + secondBullet.Type);
            textBox.Text += "\nItem 2";

            // Save the workbook
            workbook.Save("BulletValuePropertyTypeDemo.xlsx");
        }
    }
}
```

### See Also

* enum [BulletType](../../bullettype/)
* class [BulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


