---
title: "RenderingWatermark.VAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingWatermark. Obtiene o establece la alineación vertical de la marca de agua respecto a la página"
type: docs
url: /es/net/aspose.cells.rendering/renderingwatermark/valignment/
---
## RenderingWatermark.VAlignment property

Obtiene o establece la alineación vertical de la marca de agua respecto a la página.

```csharp
public TextAlignmentType VAlignment { get; set; }
```

### Observaciones

Solo Top, Center, Bottom son válidos. El predeterminado es Top.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyVAlignmentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Watermark VAlignment Demo");

            // Crea opciones de guardado PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Crear y configurar marca de agua con diferentes configuraciones de VAlignment
            RenderingFont font = new RenderingFont("Arial", 48)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };

            // Crear marca de agua con alineación vertical establecida en Center
            RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
            {
                VAlignment = TextAlignmentType.Center,
                HAlignment = TextAlignmentType.Center,
                Opacity = 0.5f
            };
            pdfSaveOptions.Watermark = watermark;

            // Guardar el libro de trabajo con marca de agua
            workbook.Save("WatermarkVAlignmentDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


