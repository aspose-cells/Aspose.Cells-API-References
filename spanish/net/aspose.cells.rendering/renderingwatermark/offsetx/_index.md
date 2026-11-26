---
title: "RenderingWatermark.OffsetX"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingWatermark. Obtiene o establece el valor de desplazamiento a HAlignment"
type: docs
url: /es/net/aspose.cells.rendering/renderingwatermark/offsetx/
---
## RenderingWatermark.OffsetX property

Obtiene o establece el valor de desplazamiento a [`HAlignment`](../halignment/)

```csharp
public float OffsetX { get; set; }
```

### Ejemplos

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

### Ver también

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


