---
title: "Classe TilePicOption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.TilePicOption. Rappresenta l'immagine a mosaico come texture"
type: docs
url: /it/net/aspose.cells.drawing/tilepicoption/
---
## TilePicOption class

Rappresenta l'immagine a piastrelle come trama.

```csharp
public class TilePicOption
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TilePicOption](tilepicoption/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing/tilepicoption/alignmenttype/) { get; set; } | Ottiene o imposta l'allineamento per la piastrellatura. |
| [MirrorType](../../aspose.cells.drawing/tilepicoption/mirrortype/) { get; set; } | Ottiene o imposta il tipo di specchio per la piastrellatura. |
| [OffsetX](../../aspose.cells.drawing/tilepicoption/offsetx/) { get; set; } | Ottiene o imposta lo spostamento X per l'immagine a piastrellatura. |
| [OffsetY](../../aspose.cells.drawing/tilepicoption/offsety/) { get; set; } | Ottiene o imposta lo spostamento Y per l'immagine a piastrellatura. |
| [ScaleX](../../aspose.cells.drawing/tilepicoption/scalex/) { get; set; } | Ottiene o imposta la scala X per l'immagine a piastrellatura. |
| [ScaleY](../../aspose.cells.drawing/tilepicoption/scaley/) { get; set; } | Ottiene o imposta la scala Y per l'immagine a piastrellatura. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTilePicOptionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un grafico per la dimostrazione
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Imposta il tipo di riempimento a texture
            chart.ChartArea.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Texture;

            // Carica l'immagine di esempio (sostituisci con il percorso reale)
            byte[] imageData = File.ReadAllBytes("sample.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Crea e configura TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            tileOptions.ScaleX = 50;
            tileOptions.ScaleY = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = tileOptions;

            // Salva la cartella di lavoro
            workbook.Save("TilePicOptionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


