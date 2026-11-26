---
title: "ImageOrPrintOptions.EmbededImageNameInSvg"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Indique el nombre de archivo de la imagen incrustada en svg. Debe ser una ruta completa con directorio, como cxpsEmbedded"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/
---
## ImageOrPrintOptions.EmbededImageNameInSvg property

Indique el nombre de archivo de la imagen incrustada en svg. Esto debe ser la ruta completa con el directorio, como "c:\\xpsEmbedded"

```csharp
[Obsolete("Images are now always embedded in Svg with base64 format, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EmbededImageNameInSvg { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, elimine esta propiedad porque las imágenes ahora siempre se incrustan en Svg con formato base64. Esta propiedad será eliminada 12 meses después, a partir de abril de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmbededImageNameInSvgDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Genere una imagen simple en memoria y añádala a la hoja de cálculo
            byte[] redPngBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            worksheet.Pictures.Add(0, 0, new MemoryStream(redPngBytes));

            // Cree opciones de renderizado de imagen con formato SVG
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Svg
            };

            // Muestre la ruta actual de la imagen incrustada
            Console.WriteLine("Initial EmbededImageNameInSvg: " + options.EmbededImageNameInSvg);

            // Configure el nuevo directorio de imágenes incrustadas
            string imageDir = "svg_embedded_images/";
            options.EmbededImageNameInSvg = imageDir;
            Directory.CreateDirectory(imageDir);

            // Renderice la hoja de cálculo a SVG con las opciones configuradas
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "worksheet_output.svg");

            Console.WriteLine("Generated SVG with embedded images in: " + Path.GetFullPath(imageDir));
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


