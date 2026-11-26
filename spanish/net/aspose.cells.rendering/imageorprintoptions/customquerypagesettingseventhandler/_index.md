---
title: "ImageOrPrintOptions.CustomQueryPageSettingsEventHandler"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. El cliente puede controlar la configuración de página de la impresora al imprimir cada página usando este EventHandler"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/
---
## ImageOrPrintOptions.CustomQueryPageSettingsEventHandler property

El cliente puede controlar la configuración de página de la impresora al imprimir cada página usando este EventHandler

```csharp
public QueryPageSettingsEventHandler CustomQueryPageSettingsEventHandler { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyCustomQueryPageSettingsEventHandlerDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";

            try
            {
                // Crear una instancia de ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Mostrar algunas de las propiedades disponibles
                Console.WriteLine("Current HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("Current VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // Demostrar la configuración de algunas propiedades
                options.HorizontalResolution = 300;
                options.VerticalResolution = 300;
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Verificar que las propiedades están configuradas
                Console.WriteLine("Updated HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("Updated VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("Updated ImageType: " + options.ImageType);

                // Crear un SheetRender para demostrar el renderizado
                SheetRender renderer = new SheetRender(worksheet, options);

                // Guarda el libro de trabajo
                workbook.Save("CustomQueryPageSettingsEventHandlerDemo.xlsx");

                Console.WriteLine("ImageOrPrintOptions demonstration completed");
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


