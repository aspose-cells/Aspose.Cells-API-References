---
title: "RenderingWatermark.Rotation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RenderingWatermark. Ottiene o imposta la rotazione della filigrana in gradi"
type: docs
url: /it/net/aspose.cells.rendering/renderingwatermark/rotation/
---
## RenderingWatermark.Rotation property

Ottiene o imposta la rotazione della filigrana in gradi.

```csharp
public float Rotation { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyRotationDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data for watermark demo");

            // Crea carattere per la filigrana
            RenderingFont font = new RenderingFont("Arial", 72);
            font.Color = Color.FromArgb(128, 0, 0, 255);
            font.Bold = true;

            // Crea filigrana con rotazione
            RenderingWatermark watermark = new RenderingWatermark("ROTATED WATERMARK", font);
            watermark.Rotation = 45; // 45 degree rotation
            watermark.Opacity = 0.5f;
            watermark.IsBackground = true;

            // Imposta opzioni di salvataggio PDF con filigrana
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Salva con filigrana
            workbook.Save("WatermarkRotationDemo.pdf", options);
        }
    }
}
```

### Vedi anche

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


