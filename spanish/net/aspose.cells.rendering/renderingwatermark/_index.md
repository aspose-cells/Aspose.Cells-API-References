---
title: "Clase RenderingWatermark"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.RenderingWatermark. Marca de agua para renderizado"
type: docs
url: /es/net/aspose.cells.rendering/renderingwatermark/
---
## RenderingWatermark class

Marca de agua para renderizado.

```csharp
public class RenderingWatermark
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [RenderingWatermark](renderingwatermark/#constructor)(byte[]) | Crea una instancia de marca de agua de imagen. |
| [RenderingWatermark](renderingwatermark/#constructor_1)(string, RenderingFont) | Crea una instancia de marca de agua de texto. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Font](../../aspose.cells.rendering/renderingwatermark/font/) { get; } | Obtiene la fuente de la marca de agua. |
| [HAlignment](../../aspose.cells.rendering/renderingwatermark/halignment/) { get; set; } | Obtiene o establece la alineación horizontal de la marca de agua respecto a la página. |
| [Image](../../aspose.cells.rendering/renderingwatermark/image/) { get; } | Obtiene la imagen de la marca de agua. |
| [IsBackground](../../aspose.cells.rendering/renderingwatermark/isbackground/) { get; set; } | Indica si la marca de agua se coloca detrás del contenido de la página. |
| [OffsetX](../../aspose.cells.rendering/renderingwatermark/offsetx/) { get; set; } | Obtiene o establece el valor de desplazamiento a [`HAlignment`](./halignment/) |
| [OffsetY](../../aspose.cells.rendering/renderingwatermark/offsety/) { get; set; } | Obtiene o establece el valor de desplazamiento a [`VAlignment`](./valignment/) |
| [Opacity](../../aspose.cells.rendering/renderingwatermark/opacity/) { get; set; } | Obtiene o establece la opacidad de la marca de agua en el rango [0, 1]. |
| [Rotation](../../aspose.cells.rendering/renderingwatermark/rotation/) { get; set; } | Obtiene o establece la rotación de la marca de agua en grados. |
| [ScaleToPagePercent](../../aspose.cells.rendering/renderingwatermark/scaletopagepercent/) { get; set; } | Obtiene o establece la escala relativa a la página objetivo en porcentaje. |
| [Text](../../aspose.cells.rendering/renderingwatermark/text/) { get; } | Obtiene el texto de la marca de agua. |
| [VAlignment](../../aspose.cells.rendering/renderingwatermark/valignment/) { get; set; } | Obtiene o establece la alineación vertical de la marca de agua respecto a la página. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class RenderingWatermarkDemo
    {
        public static void RenderingWatermarkExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample worksheet.");

            // Crea una fuente para la marca de agua
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Crea una marca de agua a partir del texto y la fuente especificada
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font);

            // Establece propiedades para la marca de agua
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 30;
            watermark.Opacity = 0.6f;
            watermark.ScaleToPagePercent = 50;
            watermark.IsBackground = true;

            // Especifica la marca de agua para renderizar a PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Guarde el libro de trabajo como PDF con la marca de agua
            workbook.Save("output_watermark.pdf", options);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


