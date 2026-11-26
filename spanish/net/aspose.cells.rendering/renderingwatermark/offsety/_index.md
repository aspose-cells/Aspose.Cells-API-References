---
title: "RenderingWatermark.OffsetY"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingWatermark. Obtiene o establece el valor de desplazamiento a VAlignment"
type: docs
url: /es/net/aspose.cells.rendering/renderingwatermark/offsety/
---
## RenderingWatermark.OffsetY property

Obtiene o establece el valor de desplazamiento a [`VAlignment`](../valignment/)

```csharp
public float OffsetY { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyOffsetYDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("OffsetY Demo");

            // Crear fuente de marca de agua
            RenderingFont font = new RenderingFont("Arial", 24)
            {
                Color = Color.Red,
                Bold = true
            };

            // Crear marca de agua con diferentes valores de OffsetY
            RenderingWatermark watermark = new RenderingWatermark("VERTICAL OFFSET", font)
            {
                Rotation = 0,
                Opacity = 0.3f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 100 // Demonstrating OffsetY property
            };

            // Establecer opciones de guardado con marca de agua
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Guardar con desplazamiento de marca de agua
            workbook.Save("WatermarkOffsetYDemo.pdf", options);
        }
    }
}
```

### Ver también

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


