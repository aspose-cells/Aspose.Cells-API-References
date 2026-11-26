---
title: "ImageOrPrintOptions.ImageType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece el formato de las imágenes generadas. valor predeterminado PNG"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/imagetype/
---
## ImageOrPrintOptions.ImageType property

Obtiene o establece el formato de las imágenes generadas. Valor predeterminado: PNG.

```csharp
public virtual ImageType ImageType { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test SVG Image");

            // Establecer opciones de guardado HTML con tipo de imagen SVG
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = ImageType.Svg;
            options.ExportActiveWorksheetOnly = true;

            // Guarda el libro de trabajo como HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, options);

            Console.WriteLine("File saved with SVG images: " + outputPath);
        }
    }
}
```

### Ver también

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


