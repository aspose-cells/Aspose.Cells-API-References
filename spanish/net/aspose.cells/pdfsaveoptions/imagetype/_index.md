---
title: "PdfSaveOptions.ImageType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Representa el tipo de imagen al convertir el gráfico y la forma"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/imagetype/
---
## PdfSaveOptions.ImageType property

Representa el tipo de imagen al convertir el gráfico y la forma.

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ImageType { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, Chart y Shape siempre se renderizan como elementos vectoriales (p. ej., punto, línea) para mejorar la calidad de renderizado. Esta propiedad será eliminada 12 meses después desde junio de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing.Imaging;

    public class PdfSaveOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo con algunos datos
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for PDF Export";
            worksheet.Cells["A2"].Value = "Demonstrating ImageType Property";

            try
            {
                // Crea opciones de guardado PDF
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Mostrar el valor predeterminado de ImageType
                Console.WriteLine("Default ImageType: " + saveOptions.ImageType);

                // Establecer un valor diferente de ImageType
                saveOptions.ImageType = ImageFormat.Png;
                Console.WriteLine("Updated ImageType: " + saveOptions.ImageType);

                // Guardar el libro de trabajo como PDF con el ImageType especificado
                workbook.Save("ImageTypeDemo.pdf", saveOptions);

                Console.WriteLine("PDF saved with ImageType setting applied.");
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


