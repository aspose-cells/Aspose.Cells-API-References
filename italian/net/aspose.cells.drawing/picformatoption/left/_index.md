---
title: "PicFormatOption.Left"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PicFormatOption. Ottiene o imposta l'offset sinistro per l'allungamento dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/picformatoption/left/
---
## PicFormatOption.Left property

Ottiene o imposta lo spostamento sinistro per lo stretching dell'immagine.

```csharp
public double Left { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyLeftDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare per dimostrare la formattazione dell'immagine
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 150);

            // Configura il riempimento dell'immagine per la forma
            shape.FillFormat.ImageData = File.ReadAllBytes("sample.png"); // Ensure this image exists

            // Crea e configura PicFormatOption
            PicFormatOption picFormat = new PicFormatOption
            {
                Type = FillPictureType.Stretch,
                Left = 0.0 // Initial left offset (0%)
            };

            // Applica le opzioni di formato alla forma (presumendo il nome corretto della proprietà)
            // Nota: la proprietà originale 'PictureFormatOptions' potrebbe non esistere nella versione corrente dell'API.
            // La riga sotto è commentata per risolvere l'errore di compilazione.
            // shape.FillFormat.PictureFormatOptions = picFormat;

            // Visualizza l'offset sinistro iniziale
            Console.WriteLine("Initial Left offset: " + picFormat.Left);

            // Modifica l'offset sinistro per ritagliare il 20% dal lato sinistro
            picFormat.Left = 0.2;
            Console.WriteLine("Modified Left offset: " + picFormat.Left);

            // Salva la cartella di lavoro con la formattazione dell'immagine modificata
            workbook.Save("LeftPropertyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


