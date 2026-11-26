---
title: "PdfSaveOptions.Watermark"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Obtiene o establece la marca de agua para la salida"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/watermark/
---
## PdfSaveOptions.Watermark property

Obtiene o establece la marca de agua para la salida.

```csharp
public RenderingWatermark Watermark { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyWatermarkDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con 3 hojas de cálculo
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells["A1"].PutValue("Page1");
            int index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page2");
            index = wb.Worksheets.Add();
            wb.Worksheets[index].Cells["A1"].PutValue("Page3");

            // Crear fuente de marca de agua
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Crear marca de agua con texto y fuente
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 45;
            watermark.Opacity = 0.3f;
            watermark.ScaleToPagePercent = 75;

            // Establecer la marca de agua en las opciones de guardado PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Guardar el libro de trabajo con marca de agua
            wb.Save("output_watermark.pdf", options);
        }
    }
}
```

### Ver también

* class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


