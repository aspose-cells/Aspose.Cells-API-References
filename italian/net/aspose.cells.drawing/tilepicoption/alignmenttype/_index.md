---
title: "TilePicOption.AlignmentType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TilePicOption. Ottiene o imposta l'allineamento per il tiling"
type: docs
url: /it/net/aspose.cells.drawing/tilepicoption/alignmenttype/
---
## TilePicOption.AlignmentType property

Ottiene o imposta l'allineamento per la piastrellatura.

```csharp
public RectangleAlignmentType AlignmentType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyAlignmentTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma rettangolare per dimostrare il mosaico
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 300);

            // Configura il formato di riempimento per utilizzare l'immagine a mosaico
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // Crea e configura TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // Visualizza il valore iniziale di AlignmentType
            Console.WriteLine("Current AlignmentType: " + tileOptions.AlignmentType);

            // Imposta l'allineamento a TopRight
            tileOptions.AlignmentType = RectangleAlignmentType.TopRight;
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;

            // Applica le opzioni di mosaico al riempimento della forma
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Carica l'immagine di esempio (punto rosso 1x1 pixel)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Salvare la cartella di lavoro modificata
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo.xlsx");

            // Cambia l'allineamento a BottomLeft e salva un'altra versione
            tileOptions.AlignmentType = RectangleAlignmentType.BottomLeft;
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo_BottomLeft.xlsx");
        }
    }
}
```

### Vedi anche

* enum [RectangleAlignmentType](../../rectanglealignmenttype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


