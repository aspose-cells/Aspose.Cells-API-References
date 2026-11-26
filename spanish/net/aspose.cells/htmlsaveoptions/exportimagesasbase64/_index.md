---
title: "HtmlSaveOptions.ExportImagesAsBase64"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportimagesasbase64/
---
## HtmlSaveOptions.ExportImagesAsBase64 property

Especifica si las imágenes se guardan en formato Base64 en HTML, MHTML o EPUB.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Observaciones

Cuando esta propiedad se establece en true, los datos de la imagen se exportan directamente en los elementos img y no se crean archivos separados.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una imagen a la hoja de cálculo
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Establecer ExportImagesAsBase64 en true para incrustar imágenes como cadenas base64
            saveOptions.ExportImagesAsBase64 = true;
            
            // Guardar el libro de trabajo como HTML con imágenes incrustadas
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML with embedded images saved successfully.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


