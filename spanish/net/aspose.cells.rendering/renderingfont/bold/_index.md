---
title: "RenderingFont.Bold"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingFont. Obtiene o establece negrita para la fuente"
type: docs
url: /es/net/aspose.cells.rendering/renderingfont/bold/
---
## RenderingFont.Bold property

Obtiene o establece negrita para la fuente.

```csharp
public bool Bold { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontPropertyBoldDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Bold Font Example");

            // Crear un estilo para la celda
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Crear opciones de guardado PDF con marca de agua que muestra fuente en negrita
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Crear fuente de renderizado con propiedad en negrita
            RenderingFont font = new RenderingFont("Arial", 36)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };
            
            // Crear marca de agua con fuente en negrita
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Opacity = 0.3f
            };
            pdfSaveOptions.Watermark = watermark;

            // Guarda el libro de trabajo
            workbook.Save("BoldFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


