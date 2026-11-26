---
title: "RenderingWatermark.Font"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingWatermark. Obtiene la fuente de la marca de agua"
type: docs
url: /es/net/aspose.cells.rendering/renderingwatermark/font/
---
## RenderingWatermark.Font property

Obtiene la fuente de la marca de agua.

```csharp
public RenderingFont Font { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear una fuente de renderizado y establecer propiedades iniciales
            RenderingFont font = new RenderingFont("Arial", 24);
            
            // Crear una marca de agua de texto con la fuente de renderizado
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            
            // Mostrar propiedades de fuente iniciales
            Console.WriteLine("Initial Font Name: " + watermark.Font.Name);
            Console.WriteLine("Initial Font Size: " + watermark.Font.Size);
            Console.WriteLine("Initial Bold Status: " + watermark.Font.Bold);
            
            // Modificar propiedades de fuente a través de la referencia RenderingFont
            font.Bold = true;
            
            // Mostrar propiedades de fuente actualizadas de la marca de agua
            Console.WriteLine("\nUpdated Font Name: " + watermark.Font.Name);
            Console.WriteLine("Updated Font Size: " + watermark.Font.Size);
            Console.WriteLine("Updated Bold Status: " + watermark.Font.Bold);
            
            // Configurar propiedades de visualización de la marca de agua
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            watermark.IsBackground = true;
            
            // Crear opciones de guardado PDF y asignar marca de agua
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Watermark = watermark;
            
            // Guardar el libro de trabajo con PDF marcado para mostrar cambios de fuente
            workbook.Save("RenderingWatermarkFontDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


