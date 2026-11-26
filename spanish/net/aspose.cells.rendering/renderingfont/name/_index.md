---
title: "RenderingFont.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingFont. Obtiene el nombre de la fuente"
type: docs
url: /es/net/aspose.cells.rendering/renderingfont/name/
---
## RenderingFont.Name property

Obtiene el nombre de la fuente.

```csharp
public string Name { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingFontPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crea opciones de guardado PDF
            PdfSaveOptions options = new PdfSaveOptions();

            // Crea una fuente de renderizado inicial con "Arial"
            RenderingFont fontArial = new RenderingFont("Arial", 16);
            Console.WriteLine("Initial font name: " + fontArial.Name);

            // Crea una marca de agua con la fuente inicial
            RenderingWatermark watermark = new RenderingWatermark("Confidential", fontArial);
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            options.Watermark = watermark;

            // Guarda con la marca de agua de fuente inicial
            workbook.Save("WatermarkInitial.pdf", options);

            // Crea una nueva fuente de renderizado con "Times New Roman"
            RenderingFont fontTimesNewRoman = new RenderingFont("Times New Roman", 16);
            Console.WriteLine("\nModified font name: " + fontTimesNewRoman.Name);

            // Actualiza la marca de agua con la nueva fuente
            RenderingWatermark updatedWatermark = new RenderingWatermark("Confidential", fontTimesNewRoman);
            updatedWatermark.Opacity = 0.5f;
            updatedWatermark.Rotation = 45;
            options.Watermark = updatedWatermark;

            // Guarda con la marca de agua de fuente modificada
            workbook.Save("WatermarkModified.pdf", options);
        }
    }
}
```

### Ver también

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


