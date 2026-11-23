---
title: "RenderingWatermark.OffsetX"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété RenderingWatermark. Obtient ou définit la valeur de décalage pour HAlignment"
type: docs
url: /fr/net/aspose.cells.rendering/renderingwatermark/offsetx/
---
## RenderingWatermark.OffsetX property

Obtient ou définit la valeur de décalage pour [`HAlignment`](../halignment/)

```csharp
public float OffsetX { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyOffsetXDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Sample Data");

            RenderingFont font = new RenderingFont("Arial", 24)
            {
                Color = Color.Red,
                Bold = true
            };

            RenderingWatermark watermark = new RenderingWatermark("DEMO WATERMARK", font)
            {
                Rotation = 45,
                Opacity = 0.3f,
                IsBackground = true,
                OffsetX = 100,  // Demonstrating OffsetX property
                OffsetY = 50
            };

            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            workbook.Save("WatermarkWithOffsetX.pdf", options);
        }
    }
}
```

### Voir aussi

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


