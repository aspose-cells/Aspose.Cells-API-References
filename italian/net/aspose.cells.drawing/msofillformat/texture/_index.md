---
title: "MsoFillFormat.Texture"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFillFormat. Restituisce il tipo di riempimento a trama"
type: docs
url: /it/net/aspose.cells.drawing/msofillformat/texture/
---
## MsoFillFormat.Texture property

Ottiene il tipo di riempimento texture.

```csharp
public TextureType Texture { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare per dimostrare la formattazione del riempimento
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Ottieni il formato di riempimento
            MsoFillFormat fillFormat = rectangle.FillFormat;

            try
            {
                // Visualizza il tipo di trama corrente (proprietà di sola lettura)
                TextureType currentTexture = fillFormat.Texture;
                Console.WriteLine("Current Texture Type: " + currentTexture);

                // Imposta alcuni dati immagine per potenzialmente cambiare la trama
                // Questo dimostra come la trama possa essere influenzata dai dati immagine
                byte[] sampleImageData = new byte[] { 0x89, 0x50, 0x4E, 0x47 }; // PNG header
                fillFormat.ImageData = sampleImageData;

                // Visualizza nuovamente il tipo di trama dopo aver impostato i dati immagine
                TextureType updatedTexture = fillFormat.Texture;
                Console.WriteLine("Texture Type after setting image data: " + updatedTexture);

                // Salva la cartella di lavoro
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

### Vedi anche

* enum [TextureType](../../texturetype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


