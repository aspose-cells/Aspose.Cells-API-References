---
title: "TextureFill.PicFormatOption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextureFill. Ottiene o imposta l'opzione del formato immagine"
type: docs
url: /it/net/aspose.cells.drawing/texturefill/picformatoption/
---
## TextureFill.PicFormatOption property

Ottiene o imposta l'opzione del formato immagine.

```csharp
public PicFormatOption PicFormatOption { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextureFillPropertyPicFormatOptionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare
            var shape = worksheet.Shapes.AddRectangle(0, 0, 100, 300, 200, 400);

            // Configura il riempimento texture
            shape.Fill.FillType = FillType.Texture;
            TextureFill textureFill = shape.Fill.TextureFill;

            // Imposta una texture definita dall'utente con un'immagine minima 1x1 pixel
            // TextureType.UserDefined non è disponibile, rimossa l'assegnazione non valida
            textureFill.ImageData = new byte[] { 
                0x89, 0x50, 0x4E, 0x47, 0x0D, 0x0A, 0x1A, 0x0A, 0x00, 0x00, 0x00, 0x0D, 0x49, 0x48, 0x44, 0x52,
                0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x08, 0x02, 0x00, 0x00, 0x00, 0x90, 0x77, 0x53,
                0xDE, 0x00, 0x00, 0x00, 0x01, 0x73, 0x52, 0x47, 0x42, 0x00, 0xAE, 0xCE, 0x1C, 0xE9, 0x00, 0x00,
                0x00, 0x04, 0x67, 0x41, 0x4D, 0x41, 0x00, 0x00, 0xB1, 0x8F, 0x0B, 0xFC, 0x61, 0x05, 0x00, 0x00,
                0x00, 0x09, 0x70, 0x48, 0x59, 0x73, 0x00, 0x00, 0x0E, 0xC3, 0x00, 0x00, 0x0E, 0xC3, 0x01, 0xC7,
                0x6F, 0xA8, 0x64, 0x00, 0x00, 0x00, 0x18, 0x49, 0x44, 0x41, 0x54, 0x18, 0x57, 0x63, 0x60, 0x18,
                0x05, 0xA3, 0x60, 0x14, 0x8C, 0x82, 0x51, 0x30, 0x0A, 0x46, 0xC1, 0x28, 0x00, 0x00, 0x01, 0xAD,
                0x00, 0x01, 0x8C, 0xF8, 0x2B, 0xD4, 0x00, 0x00, 0x00, 0x00, 0x49, 0x45, 0x4E, 0x44, 0xAE, 0x42,
                0x60, 0x82 
            };

            // Abilita il tiling e mostra le opzioni di formato
            textureFill.IsTiling = true;

            // Visualizza lo stato iniziale di PicFormatOption
            Console.WriteLine("Initial PicFormatOption: " + (textureFill.PicFormatOption != null ? "Configured" : "Null"));

            // Crea e applica nuove opzioni di formato
            textureFill.PicFormatOption = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Scale = 0.25,
                Left = 15,    // Corrected from LeftOffset
                Top = 15,     // Corrected from TopOffset
                // Le proprietà ScaleX e ScaleY non esistono - rimosse
            };

            // Verifica l'aggiornamento della proprietà
            Console.WriteLine("Updated PicFormatOption Type: " + textureFill.PicFormatOption.Type);

            // Salva con modello di piastrellatura modificato
            workbook.Save("TextureFillPicFormatOptionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PicFormatOption](../../picformatoption/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


