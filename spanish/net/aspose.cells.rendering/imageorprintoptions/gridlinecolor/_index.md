---
title: "ImageOrPrintOptions.GridlineColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece el color de la cuadrícula"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/gridlinecolor/
---
## ImageOrPrintOptions.GridlineColor property

Obtiene o establece el color de la línea de cuadrícula.

```csharp
public Color GridlineColor { get; set; }
```

### Observaciones

Ignorará la configuración del color de la línea de cuadrícula en el archivo fuente.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue algunos datos de muestra para que la hoja de cálculo tenga contenido
            worksheet.Cells["A1"].PutValue("Demo for GridlineColor property");

            try
            {
                // Cree una instancia de ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Muestre el valor actual de GridlineColor (solo lectura o lectura/escritura)
                // Se asume que el tipo de la propiedad es System.Drawing.Color
                Console.WriteLine("Current GridlineColor: " + options.GridlineColor);

                // Opcionalmente renderice la hoja a una imagen para ver el efecto del color de cuadrícula predeterminado
                // (No es necesario cambiar el valor; solo demostramos su uso.)
                SheetRender renderer = new SheetRender(worksheet, options);
                renderer.ToImage(0, "GridlineColorDemo.png");

                // Guardar el libro de trabajo (opcional)
                workbook.Save("GridlineColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


