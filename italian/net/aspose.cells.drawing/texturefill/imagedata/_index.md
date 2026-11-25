---
title: "TextureFill.ImageData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextureFill. Ottiene e imposta i dati immagine del riempimento"
type: docs
url: /it/net/aspose.cells.drawing/texturefill/imagedata/
---
## TextureFill.ImageData property

Ottiene e imposta i dati immagine del riempimento.

```csharp
public byte[] ImageData { get; set; }
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
    public class TextureFillPropertyImageDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta il tipo di riempimento texture
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;

            // Carica i dati dell'immagine
            byte[] imageData = File.ReadAllBytes("texture.png");

            // Imposta i dati immagine per il riempimento texture
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Salva la cartella di lavoro
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


