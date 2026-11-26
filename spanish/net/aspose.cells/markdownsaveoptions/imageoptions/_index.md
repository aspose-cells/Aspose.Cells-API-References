---
title: "MarkdownSaveOptions.ImageOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. Obtenga el objeto ImageOrPrintOptions antes de exportar"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/imageoptions/
---
## MarkdownSaveOptions.ImageOptions property

Obtenga el objeto ImageOrPrintOptions antes de exportar

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class MarkdownSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para que el ejemplo tenga sentido
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Image Options Demo";

            try
            {
                // Crear una instancia de MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Acceder a la propiedad ImageOptions (solo lectura)
                ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;

                // Mostrar los valores actuales de las propiedades de ImageOptions
                Console.WriteLine("ImageOptions properties:");
                Console.WriteLine($"HorizontalResolution: {imageOptions.HorizontalResolution}");
                Console.WriteLine($"VerticalResolution: {imageOptions.VerticalResolution}");
                Console.WriteLine($"ImageType: {imageOptions.ImageType}");
                Console.WriteLine($"Quality: {imageOptions.Quality}");
                Console.WriteLine($"Transparent: {imageOptions.Transparent}");

                // Guardar el libro de trabajo con las opciones actuales
                workbook.Save("ImageOptionsDemo.md", saveOptions);

                Console.WriteLine("Markdown file saved successfully with ImageOptions demonstrated.");
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

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


