---
title: "RenderingFont.Color"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingFont. Obtiene o establece el color de la fuente"
type: docs
url: /es/net/aspose.cells.rendering/renderingfont/color/
---
## RenderingFont.Color property

Obtiene o establece color para la fuente.

```csharp
public Color Color { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Testing font color property");

            RenderingFont font = new RenderingFont("Arial", 16);
            font.Color = System.Drawing.Color.Red;
            font.Bold = true;

            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = new RenderingWatermark("COLOR DEMO", font)
            {
                Opacity = 0.5f,
                IsBackground = true
            };

            workbook.Save("FontColorDemo.pdf", options);
        }
    }
}
```

### Ver también

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


