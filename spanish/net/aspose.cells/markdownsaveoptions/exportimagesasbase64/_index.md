---
title: "MarkdownSaveOptions.ExportImagesAsBase64"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. Especifica si las imágenes se guardan en formato Base64 en Markdown. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/exportimagesasbase64/
---
## MarkdownSaveOptions.ExportImagesAsBase64 property

Especifica si las imágenes se guardan en formato Base64 en Markdown. El valor predeterminado es verdadero.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Observaciones

Cuando esta propiedad se establece en true, los datos de la imagen se exportan directamente en los elementos img y no se crean archivos separados.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra y una imagen
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("With Image");

            // Agregar una imagen a la hoja de cálculo
            int imageIndex = worksheet.Pictures.Add(1, 1, "sample.png");

            try
            {
                // Crear una instancia de MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Mostrar el valor predeterminado de ExportImagesAsBase64
                Console.WriteLine("Default ExportImagesAsBase64 value: " + saveOptions.ExportImagesAsBase64);

                // Establecer ExportImagesAsBase64 a false para demostrar la propiedad
                saveOptions.ExportImagesAsBase64 = false;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // Guardar con ExportImagesAsBase64 = false
                workbook.Save("MarkdownImagesAsFiles.md", saveOptions);

                // Establecer ExportImagesAsBase64 a true
                saveOptions.ExportImagesAsBase64 = true;
                Console.WriteLine("ExportImagesAsBase64 set to: " + saveOptions.ExportImagesAsBase64);

                // Guardar con ExportImagesAsBase64 = true
                workbook.Save("MarkdownImagesAsBase64.md", saveOptions);

                Console.WriteLine("Markdown files saved with different ExportImagesAsBase64 settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


