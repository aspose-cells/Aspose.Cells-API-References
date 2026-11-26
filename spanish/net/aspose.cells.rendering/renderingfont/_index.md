---
title: "Class RenderingFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Rendering.RenderingFont class. Fuente para renderizado"
type: docs
url: /es/net/aspose.cells.rendering/renderingfont/
---
## RenderingFont class

Fuente para renderizado.

```csharp
public class RenderingFont
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [RenderingFont](renderingfont/)(string, float) | Inicializa una nueva instancia de `RenderingFont` |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Bold](../../aspose.cells.rendering/renderingfont/bold/) { get; set; } | Obtiene o establece negrita para la fuente. |
| [Color](../../aspose.cells.rendering/renderingfont/color/) { get; set; } | Obtiene o establece color para la fuente. |
| [Italic](../../aspose.cells.rendering/renderingfont/italic/) { get; set; } | Obtiene o establece cursiva para la fuente. |
| [Name](../../aspose.cells.rendering/renderingfont/name/) { get; } | Obtiene el nombre de la fuente. |
| [Size](../../aspose.cells.rendering/renderingfont/size/) { get; } | Obtiene el tamaño de la fuente en puntos. |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingFontDemo
    {
        public static void RenderingFontExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            sheet.Cells["A1"].PutValue("Hello World!");

            // Crea un objeto RenderingFont
            RenderingFont renderingFont = new RenderingFont("Arial", 12)
            {
                Bold = true,
                Italic = true,
                Color = Color.Blue
            };

            // Crea un objeto RenderingWatermark usando el RenderingFont
            RenderingWatermark watermark = new RenderingWatermark("Sample Watermark", renderingFont)
            {
                Rotation = 45,
                ScaleToPagePercent = 100,
                Opacity = 0.5f,
                IsBackground = true,
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                OffsetX = 0,
                OffsetY = 0
            };

            // Crea PdfSaveOptions y establece la marca de agua
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Watermark = watermark,
                EmbedStandardWindowsFonts = true,
                CalculateFormula = true,
                ExportDocumentStructure = true,
                DisplayDocTitle = true
            };

            // Guarda el libro de trabajo en PDF con la marca de agua
            workbook.Save("RenderingFontExample.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


