---
title: "SvgImageOptions.ImageType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SvgImageOptions. Obtiene o establece el formato de las imágenes generadas. valor predeterminado PNG"
type: docs
url: /es/net/aspose.cells.rendering/svgimageoptions/imagetype/
---
## SvgImageOptions.ImageType property

Obtiene o establece el formato de las imágenes generadas. Valor predeterminado: PNG.

```csharp
public override ImageType ImageType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SvgImageOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra y una imagen
            worksheet.Cells["A1"].PutValue("Embedded Image Type Demonstration");
            int pictureIndex = worksheet.Pictures.Add(0, 1, "inputImage.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Crear opciones de renderizado SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Mostrar ImageType actual (predeterminado: PNG)
            Console.WriteLine("Current ImageType: " + svgOptions.ImageType);

            // Cambiar el formato de imagen para imágenes raster incrustadas
            svgOptions.ImageType = ImageType.Jpeg;

            // Guardar el contenido de la hoja de cálculo como SVG con diferentes formatos de imagen
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_jpeg.svg", stream.ToArray());
            }

            // Restablecer al formato PNG
            svgOptions.ImageType = ImageType.Png;
            
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_png.svg", stream.ToArray());
            }

            Console.WriteLine("SVG files created with different embedded image formats.");
        }
    }
}
```

### Ver también

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


