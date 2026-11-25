---
title: "TilePicOption.ScaleX"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TilePicOption. Ottiene o imposta la scala X per l'immagine a tiling"
type: docs
url: /it/net/aspose.cells.drawing/tilepicoption/scalex/
---
## TilePicOption.ScaleX property

Ottiene o imposta la scala X per l'immagine a piastrellatura.

```csharp
public double ScaleX { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TilePicOptionPropertyScaleXDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e crea un grafico
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Imposta il riempimento texture con l'immagine
            string imagePath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "texture.png");
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            
            // Dimostra la proprietà ScaleX
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50; // 50% horizontal scaling
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 75; // 75% vertical scaling

            // Salva la cartella di lavoro
            workbook.Save(Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ScaleXDemo.xlsx"));
        }
    }
}
```

### Vedi anche

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


