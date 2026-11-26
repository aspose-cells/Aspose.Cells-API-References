---
title: "RenderingWatermark.HAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingWatermark. Obtiene o establece la alineación horizontal de la marca de agua en la página"
type: docs
url: /es/net/aspose.cells.rendering/renderingwatermark/halignment/
---
## RenderingWatermark.HAlignment property

Obtiene o establece la alineación horizontal de la marca de agua respecto a la página.

```csharp
public TextAlignmentType HAlignment { get; set; }
```

### Observaciones

Solo Left, Center, Right son válidos. El predeterminado es Left.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyHAlignmentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Watermark HAlignment Demo");

            // Crea opciones de guardado PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Crear y configurar marca de agua con diferentes configuraciones de HAlignment
            RenderingFont font = new RenderingFont("Arial", 48)
            {
                Bold = true,
                Color = System.Drawing.Color.Blue
            };

            // Crear marca de agua con alineación Center
            RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.5f
            };
            pdfSaveOptions.Watermark = watermark;

            // Guardar con marca de agua centrada
            workbook.Save("WatermarkCenterAlignment.pdf", pdfSaveOptions);

            // Cambiar a alineación Left
            watermark.HAlignment = TextAlignmentType.Left;
            workbook.Save("WatermarkLeftAlignment.pdf", pdfSaveOptions);

            // Cambiar a alineación Right
            watermark.HAlignment = TextAlignmentType.Right;
            workbook.Save("WatermarkRightAlignment.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


