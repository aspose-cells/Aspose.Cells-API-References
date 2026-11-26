---
title: "ImageOrPrintOptions.Transparent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Indica si el fondo de la imagen generada debe ser transparente"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/transparent/
---
## ImageOrPrintOptions.Transparent property

Indica si el fondo de la imagen generada debe ser transparente.

```csharp
public bool Transparent { get; set; }
```

### Observaciones

El valor predeterminado es false. Eso significa que el fondo de las imágenes generadas es blanco.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTransparentDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Transparent Image Demo");
            
            // Establecer opciones de guardado HTML con imagen PNG transparente
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.ImageOptions.Transparent = true;
            options.ExportImagesAsBase64 = true;

            // Guardar el libro de trabajo con opciones de imagen transparente
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with transparent images saved successfully.");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


