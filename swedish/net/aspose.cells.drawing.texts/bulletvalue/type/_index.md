---
title: "BulletValue.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "BulletValue-egenskapen. Hämtar typen av bulletvärdet"
type: docs
url: /sv/net/aspose.cells.drawing.texts/bulletvalue/type/
---
## BulletValue.Type property

Hämtar typen av punktlistans värde.

```csharp
public abstract BulletType Type { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en textruta och hämta dess textstycken
                var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var textParagraph = textBox.TextBody.TextParagraphs[0];

                // Skapa ett tecken-bullet-värde (som ärver från BulletValue)
                var bulletValue = new CharacterBulletValue();
                bulletValue.Character = '•';

                // Visa värdet för Type-egenskapen
                Console.WriteLine("Bullet Type: " + bulletValue.Type);

                // Skapa ett bild-bullet-värde för att visa en annan typ
                var pictureBullet = new PictureBulletValue();
                Console.WriteLine("Picture Bullet Type: " + pictureBullet.Type);

                // Spara arbetsboken
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

### Se även

* enum [BulletType](../../bullettype/)
* class [BulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


