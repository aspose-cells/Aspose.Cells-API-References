---
title: "RenderingWatermark.IsBackground"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingWatermark. Indica si la marca de agua se coloca detrás del contenido de la página"
type: docs
url: /es/net/aspose.cells.rendering/renderingwatermark/isbackground/
---
## RenderingWatermark.IsBackground property

Indica si la marca de agua se coloca detrás del contenido de la página.

```csharp
public bool IsBackground { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyIsBackgroundDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Sample Content");

            // Crear marca de agua con IsBackground establecido en true
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Color = Color.LightGray
            };
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                IsBackground = true,
                Rotation = 45,
                Opacity = 0.2f
            };

            // Configurar opciones de guardado con marca de agua
            PdfSaveOptions options = new PdfSaveOptions
            {
                Watermark = watermark
            };

            // Guardar con marca de agua de fondo
            workbook.Save("WatermarkIsBackgroundDemo.pdf", options);
        }
    }
}
```

### Ver también

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


