---
title: "TilePicOption.OffsetX"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TilePicOption. Ottiene o imposta lo spostamento X per l'immagine a mosaico"
type: docs
url: /it/net/aspose.cells.drawing/tilepicoption/offsetx/
---
## TilePicOption.OffsetX property

Ottiene o imposta lo spostamento X per l'immagine a piastrellatura.

```csharp
public double OffsetX { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TilePicOptionPropertyOffsetXDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare per dimostrare il mosaico
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Configura il formato di riempimento per utilizzare l'immagine a mosaico
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // Crea e configura TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // Leggi il valore iniziale di OffsetX
            Console.WriteLine("Current OffsetX value: " + tileOptions.OffsetX);

            // Imposta il nuovo offset X per il modello a mosaico
            tileOptions.OffsetX = 15.5;

            // Applica le opzioni di mosaico al riempimento della forma
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Carica un'immagine minima di 1x1 pixel (punto rosso)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Salvare la cartella di lavoro modificata
            workbook.Save("TilePicOptionPropertyOffsetXDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


