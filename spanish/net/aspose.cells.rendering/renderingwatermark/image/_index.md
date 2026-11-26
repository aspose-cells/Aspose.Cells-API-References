---
title: "RenderingWatermark.Image"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RenderingWatermark. Obtiene la imagen de la marca de agua"
type: docs
url: /es/net/aspose.cells.rendering/renderingwatermark/image/
---
## RenderingWatermark.Image property

Obtiene la imagen de la marca de agua.

```csharp
public byte[] Image { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System.IO;

    public class RenderingWatermarkPropertyImageDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cargar datos de imagen desde el archivo
            byte[] originalImage = File.ReadAllBytes("watermark.png");

            // Crear marca de agua basada en imagen con la imagen inicial
            RenderingWatermark watermark = new RenderingWatermark(originalImage);
            Console.WriteLine("Initial image size: " + watermark.Image.Length + " bytes");

            // Modificar propiedades de la marca de agua
            watermark.Rotation = 45f;
            watermark.Opacity = 0.5f;
            watermark.ScaleToPagePercent = 75;
            watermark.IsBackground = true;
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;

            // Crear opciones de guardado PDF con marca de agua
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Watermark = watermark; // Fixed property name

            // Guardar en PDF con salida con marca de agua
            workbook.Save("WatermarkedOutput.pdf", pdfOptions);

            // Crear nueva marca de agua con una imagen diferente
            byte[] updatedImage = File.ReadAllBytes("updated_watermark.png");
            RenderingWatermark newWatermark = new RenderingWatermark(updatedImage);
            Console.WriteLine("Updated image size: " + newWatermark.Image.Length + " bytes");

            // Guardar con nueva marca de agua
            pdfOptions.Watermark = newWatermark; // Fixed property name
            workbook.Save("UpdatedWatermark.pdf", pdfOptions);
        }
    }
}
```

### Ver también

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


