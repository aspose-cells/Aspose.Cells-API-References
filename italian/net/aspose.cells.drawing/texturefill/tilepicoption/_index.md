---
title: "TextureFill.TilePicOption"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextureFill. Ottiene o imposta l'opzione dell'immagine a piastrelle"
type: docs
url: /it/net/aspose.cells.drawing/texturefill/tilepicoption/
---
## TextureFill.TilePicOption property

Ottiene o imposta l'opzione di immagine a piastrelle.

```csharp
public TilePicOption TilePicOption { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TextureFillPropertyTilePicOptionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Imposta il riempimento texture con l'immagine
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            byte[] imageData = File.ReadAllBytes("texture.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Configura le opzioni delle piastrelle
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.OffsetX = 10;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.OffsetY = 10;

            // Salva la cartella di lavoro
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TilePicOption](../../tilepicoption/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


