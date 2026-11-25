---
title: "PicFormatOption.Scale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PicFormatOption. Ottiene o imposta quanto l'immagine si impila e si scala con"
type: docs
url: /it/net/aspose.cells.drawing/picformatoption/scale/
---
## PicFormatOption.Scale property

Ottiene o imposta il numero di stack dell'immagine e la scala associata.

```csharp
public double Scale { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO; // Added to resolve Stream-related issues

    public class PicFormatOptionPropertyScaleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un array di byte di immagine BMP 1x1 pixel
            byte[] bmpBytes = new byte[]
            {
                0x42, 0x4D, 0x39, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00,
                0x28, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00,
                0x18, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00
            };

            // Aggiungi l'immagine al foglio di lavoro usando MemoryStream
            int pictureIndex = worksheet.Pictures.Add(0, 0, new MemoryStream(bmpBytes)); // Fixed Stream conversion
            Picture picture = worksheet.Pictures[pictureIndex];

            // Configura la posizione e le dimensioni dell'immagine
            picture.UpperLeftRow = 0;
            picture.UpperLeftColumn = 0;
            picture.LowerRightRow = 1;
            picture.LowerRightColumn = 1;

            // Ottieni il riempimento texture tramite la proprietà FillFormat
            TextureFill textureFill = picture.Fill.TextureFill; // Fixed cast error
            textureFill.PicFormatOption.Type = FillPictureType.Stack;

            // Visualizza e modifica la proprietà Scale
            PicFormatOption picFormat = textureFill.PicFormatOption;
            Console.WriteLine("Current Scale value: " + picFormat.Scale);
            picFormat.Scale = 0.5;
            Console.WriteLine("Modified Scale value: " + picFormat.Scale);

            // Espandi le dimensioni della cella per visualizzare l'effetto
            worksheet.Cells.SetRowHeight(0, 100);
            worksheet.Cells.SetColumnWidth(0, 20);

            // Salva la cartella di lavoro
            workbook.Save("PropertyScaleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


