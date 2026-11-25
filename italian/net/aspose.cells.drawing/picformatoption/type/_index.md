---
title: "PicFormatOption.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PicFormatOption. Ottiene o imposta il tipo di riempimento dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/picformatoption/type/
---
## PicFormatOption.Type property

Ottiene o imposta il tipo di riempimento dell'immagine.

```csharp
public FillPictureType Type { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'immagine BMP semplice di 1x1 pixel
            byte[] bmpBytes = new byte[]
            {
                0x42, 0x4D, 0x39, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00,
                0x28, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00,
                0x18, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                0x00, 0x00, 0x00
            };

            // Aggiungi immagine al foglio di lavoro
            int pictureIndex = worksheet.Pictures.Add(0, 0, new MemoryStream(bmpBytes));
            Picture picture = worksheet.Pictures[pictureIndex];

            // Imposta la posizione e le dimensioni dell'immagine
            picture.UpperLeftRow = 0;
            picture.UpperLeftColumn = 0;
            picture.LowerRightRow = 5;
            picture.LowerRightColumn = 5;

            try
            {
                // Ottieni il PicFormatOption dal riempimento a trama dell'immagine
                PicFormatOption picFormat = picture.Fill.TextureFill.PicFormatOption;

                // Visualizza il valore corrente di Type
                Console.WriteLine("Current Type: " + picFormat.Type);

                // Imposta valori Type diversi e visualizzali
                picFormat.Type = FillPictureType.Stretch;
                Console.WriteLine("Type set to Stretch: " + picFormat.Type);

                picFormat.Type = FillPictureType.Stack;
                Console.WriteLine("Type set to Stack: " + picFormat.Type);

                picFormat.Type = FillPictureType.StackAndScale;
                Console.WriteLine("Type set to StackAndScale: " + picFormat.Type);

                // Salva la cartella di lavoro
                workbook.Save("PicFormatOptionTypeDemo.xlsx");
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

* enum [FillPictureType](../../fillpicturetype/)
* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


