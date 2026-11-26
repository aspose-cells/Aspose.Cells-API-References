---
title: "ImageOrPrintOptions.Quality"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece un valor que determina la calidad de las imágenes generadas, aplicable solo al guardar páginas en formato Jpeg. El valor predeterminado es 100"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/quality/
---
## ImageOrPrintOptions.Quality property

Obtiene o establece un valor que determina la calidad de las imágenes generadas, aplicable solo al guardar páginas en formato `Jpeg`. El valor predeterminado es 100

```csharp
public int Quality { get; set; }
```

### Observaciones

Tiene efecto solo al guardar en JPEG. El valor debe estar entre 0 y 100. El valor predeterminado es 100.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyQualityDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["C3"].PutValue(DateTime.Now);

            // Crear opciones de imagen con diferentes configuraciones de calidad
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;
            options.Quality = 100; // Highest quality

            // Renderizar la hoja de cálculo a una imagen con alta calidad
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "HighQualityOutput.jpg");

            // Cambiar la calidad para demostrar la diferencia
            options.Quality = 50; // Medium quality
            renderer.ToImage(0, "MediumQualityOutput.jpg");

            options.Quality = 10; // Low quality
            renderer.ToImage(0, "LowQualityOutput.jpg");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


