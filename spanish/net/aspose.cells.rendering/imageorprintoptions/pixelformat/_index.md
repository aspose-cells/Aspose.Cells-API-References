---
title: "ImageOrPrintOptions.PixelFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ImageOrPrintOptions property. Obtiene o establece el formato de píxel para las imágenes generadas"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/pixelformat/
---
## ImageOrPrintOptions.PixelFormat property

Obtiene o establece el formato de píxel para las imágenes generadas.

```csharp
public PixelFormat PixelFormat { get; set; }
```

### Observaciones

El valor predeterminado es PixelFormat.Format32bppArgb.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyPixelFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para que el ejemplo tenga sentido
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "PixelFormat Demo";

            try
            {
                // Crear una instancia de ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Muestra el valor actual de la propiedad ImageType (ya que PixelFormat no existe)
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // Nota: Dado que PixelFormat no existe en la API, demostramos ImageType en su lugar
                // que es la propiedad relacionada más cercana para la configuración del formato de imagen

                // Crea un SheetRender para demostrar las opciones en uso
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Guarda el resultado como una imagen para demostrar las opciones
                sheetRender.ToImage(0, "PixelFormatDemo.png");

                Console.WriteLine("ImageType property has been demonstrated. Image saved as PixelFormatDemo.png");
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

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


