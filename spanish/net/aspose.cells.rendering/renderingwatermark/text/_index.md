---
title: "RenderingWatermark.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingWatermark. Obtiene el texto de la marca de agua"
type: docs
url: /es/net/aspose.cells.rendering/renderingwatermark/text/
---
## RenderingWatermark.Text property

Obtiene el texto de la marca de agua.

```csharp
public string Text { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear fuente de renderizado para el texto de la marca de agua
            RenderingFont font = new RenderingFont("Arial", 36);

            // Inicializar la marca de agua de texto con la configuración de fuente
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);

            // Mostrar el texto actual de la marca de agua
            Console.WriteLine("Watermark Text: " + watermark.Text);

            // Configurar la apariencia de la marca de agua
            watermark.Rotation = 45f;
            watermark.Opacity = 0.3f;
            watermark.IsBackground = true;
            watermark.ScaleToPagePercent = 150;

            // Aplicar la marca de agua a las opciones de guardado PDF
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark; // Fixed property name

            // Guardar en PDF para visualizar los efectos de la marca de agua
            workbook.Save("WatermarkDemo.pdf", options);
        }
    }
}
```

### Ver también

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


