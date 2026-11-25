---
title: "TilePicOption.ScaleY"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TilePicOption. Ottiene o imposta la scala Y per l'immagine a mosaico"
type: docs
url: /it/net/aspose.cells.drawing/tilepicoption/scaley/
---
## TilePicOption.ScaleY property

Ottiene o imposta la scala Y per l'immagine a piastrellatura.

```csharp
public double ScaleY { get; set; }
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
    public class TilePicOptionPropertyScaleYDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta il riempimento texture con l'immagine
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            byte[] imageData = File.ReadAllBytes("example.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
            
            // Configura le opzioni di mosaico con ScaleY
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
            
            // Salva la cartella di lavoro
            workbook.Save("TilePicOptionScaleYDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


