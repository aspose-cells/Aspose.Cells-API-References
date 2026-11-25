---
title: "TilePicOption.MirrorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TilePicOption. Ottiene o imposta il tipo di specchio per il mosaico"
type: docs
url: /it/net/aspose.cells.drawing/tilepicoption/mirrortype/
---
## TilePicOption.MirrorType property

Ottiene o imposta il tipo di specchio per la piastrellatura.

```csharp
public MirrorType MirrorType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyMirrorTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 500, 500, 500);

            // Carica dati immagine di esempio (sostituisci con il percorso reale dell'immagine)
            byte[] imageData = File.ReadAllBytes("sample.png");

            // Crea e configura l'istanza di TilePicOption
            TilePicOption tileOptions = new TilePicOption();

            // Visualizza il valore iniziale di MirrorType
            Console.WriteLine("Current MirrorType: " + tileOptions.MirrorType);

            // Configura le opzioni di piastrellatura
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;
            tileOptions.MirrorType = MirrorType.Both;

            // Applica la configurazione del tile utilizzando le proprietà corrette
            shape.Fill.FillType = FillType.Texture;
            shape.Fill.ImageData = imageData;
            shape.Fill.TextureFill.TilePicOption = tileOptions;

            // Salva la cartella di lavoro modificata
            workbook.Save("TilePicOptionMirrorTypeDemo.xlsx");

            Console.WriteLine("Updated MirrorType: " + tileOptions.MirrorType);
        }
    }
}
```

### Vedi anche

* enum [MirrorType](../../mirrortype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


