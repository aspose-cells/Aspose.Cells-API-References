---
title: "MsoFillFormat.Texture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoFillFormat-Eigenschaft. Gibt den Texturfülltyp zurück"
type: docs
url: /de/net/aspose.cells.drawing/msofillformat/texture/
---
## MsoFillFormat.Texture property

Liest den Texturfülltyp.

```csharp
public TextureType Texture { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoFillFormatPropertyTextureDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Rechteckform hinzu, um die Füllformatierung zu demonstrieren
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Hole das Füllformat
            MsoFillFormat fillFormat = rectangle.FillFormat;

            try
            {
                // Zeigen Sie den aktuellen Texturtyp an (schreibgeschützte Eigenschaft)
                TextureType currentTexture = fillFormat.Texture;
                Console.WriteLine("Current Texture Type: " + currentTexture);

                // Setzen Sie einige Bilddaten, um die Textur möglicherweise zu ändern
                // Dies demonstriert, wie die Textur durch Bilddaten beeinflusst werden kann
                byte[] sampleImageData = new byte[] { 0x89, 0x50, 0x4E, 0x47 }; // PNG header
                fillFormat.ImageData = sampleImageData;

                // Zeigen Sie den Texturtyp erneut an, nachdem Bilddaten gesetzt wurden
                TextureType updatedTexture = fillFormat.Texture;
                Console.WriteLine("Texture Type after setting image data: " + updatedTexture);

                // Speichere die Arbeitsmappe
                workbook.Save("TextureDemo.xlsx");
                Console.WriteLine("Texture demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [TextureType](../../texturetype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


