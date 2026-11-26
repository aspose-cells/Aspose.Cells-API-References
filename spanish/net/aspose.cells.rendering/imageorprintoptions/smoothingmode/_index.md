---
title: "ImageOrPrintOptions.SmoothingMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Especifica si se aplica suavizado antialiasing a líneas y curvas y a los bordes de áreas rellenas. El valor predeterminado es SmoothingMode.None"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/smoothingmode/
---
## ImageOrPrintOptions.SmoothingMode property

Especifica si se aplica suavizado (antialiasing) a líneas y curvas y a los bordes de áreas rellenas. El valor predeterminado es SmoothingMode.None

```csharp
public SmoothingMode SmoothingMode { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySmoothingModeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "ImageOrPrintOptions Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // Crear una instancia de ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Mostrar algunas de las propiedades disponibles
                Console.WriteLine("HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("ImageType: " + options.ImageType);

                // Crear un SheetRender para demostrar la propiedad
                SheetRender renderer = new SheetRender(worksheet, options);

                // Renderizar a un flujo de memoria para demostrar la funcionalidad
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Sheet rendered successfully");
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // Guarda el libro de trabajo
                workbook.Save("ImageOrPrintOptionsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


