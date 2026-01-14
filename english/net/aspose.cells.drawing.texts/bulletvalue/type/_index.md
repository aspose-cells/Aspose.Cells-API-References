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

            try
            {
                // Create a text box and get its text paragraphs
                var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var textParagraph = textBox.TextBody.TextParagraphs[0];

                // Create a character bullet value (which inherits from BulletValue)
                var bulletValue = new CharacterBulletValue();
                bulletValue.Character = '•';

                // Display the Type property value
                Console.WriteLine("Bullet Type: " + bulletValue.Type);

                // Create a picture bullet value to show different type
                var pictureBullet = new PictureBulletValue();
                Console.WriteLine("Picture Bullet Type: " + pictureBullet.Type);

                // Save the workbook
                workbook.Save("BulletValueTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* enum [BulletType](../../bullettype/)
* class [BulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


