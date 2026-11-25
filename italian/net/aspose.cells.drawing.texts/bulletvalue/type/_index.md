---
title: "BulletValue.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BulletValue. Ottiene il tipo del valore dei punti elenco"
type: docs
url: /it/net/aspose.cells.drawing.texts/bulletvalue/type/
---
## BulletValue.Type property

Ottiene il tipo del valore del punto elenco.

```csharp
public abstract BulletType Type { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea una casella di testo e ottieni i suoi paragrafi di testo
                var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var textParagraph = textBox.TextBody.TextParagraphs[0];

                // Crea un valore di punto elenco a carattere (che eredita da BulletValue)
                var bulletValue = new CharacterBulletValue();
                bulletValue.Character = '•';

                // Visualizza il valore della proprietà Type
                Console.WriteLine("Bullet Type: " + bulletValue.Type);

                // Crea un valore di punto elenco immagine per mostrare un tipo diverso
                var pictureBullet = new PictureBulletValue();
                Console.WriteLine("Picture Bullet Type: " + pictureBullet.Type);

                // Salva la cartella di lavoro
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

### Vedi anche

* enum [BulletType](../../bullettype/)
* class [BulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


