---
title: "PicFormatOption.Bottom"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PicFormatOption. Ottiene o imposta l'offset inferiore per lo stretching dell'immagine"
type: docs
url: /it/net/aspose.cells.drawing/picformatoption/bottom/
---
## PicFormatOption.Bottom property

Ottiene o imposta lo spostamento inferiore per lo stretching dell'immagine.

```csharp
public double Bottom { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PicFormatOptionPropertyBottomDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Usa un file immagine esistente (sostituisci con il percorso reale dell'immagine)
            string imagePath = "sample.jpg";

            // Aggiungi una forma rettangolare al foglio di lavoro
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 200, 200);

            // Configura il riempimento della forma per usare l'immagine di esempio
            // FillType viene dedotto impostando ImageData, che imposta il tipo su Texture
            shape.FillFormat.ImageData = File.ReadAllBytes(imagePath);
            
            // Crea e configura le opzioni del formato immagine
            PicFormatOption picFormat = new PicFormatOption();
            picFormat.Type = FillPictureType.Stretch;

            // Visualizza il valore iniziale di Bottom
            Console.WriteLine("Initial Bottom value: " + picFormat.Bottom);

            // Modifica l'offset Bottom e visualizza il nuovo valore
            picFormat.Bottom = 0.3;
            Console.WriteLine("Modified Bottom value: " + picFormat.Bottom);

            // Associa PicFormatOption al riempimento della forma (se applicabile)
            // Nota: questo passaggio potrebbe richiedere metodi specifici dell'API non mostrati nel contesto fornito
            // Per dimostrazione, PicFormatOption viene creato e configurato

            // Salva la cartella di lavoro con le modifiche applicate
            workbook.Save("PicFormatOptionBottomDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PicFormatOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


